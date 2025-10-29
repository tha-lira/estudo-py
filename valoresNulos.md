# 🧹 Valores Nulos (NaN)

### O que são

 - Representam dados faltantes em um dataset.

 - Podem aparecer por erro na coleta de dados ou preenchimento incompleto.

### 🔍 Como identificar

```
df.isnull().sum()  # Conta quantos valores nulos por coluna

df.info()          # Mostra se há colunas com nulos e seus tipos
```

### 🛠️ Como tratar

Existem **três** estratégias principais:

1️⃣ Remover nulos
   
 - Remove linhas ou colunas com valores faltantes.

 - Útil quando há poucos dados ausentes e isso não afeta a análise.
   
```
df.dropna(inplace=True)
```

2️⃣ Preencher nulos
   
 - Numéricos: média ou mediana
   
```
# Com a média (bom para dados sem muitos outliers)

df["salario"].fillna(df["salario"].mean(), inplace=True)

# Com a mediana (mais segura se há outliers)

df["salario"].fillna(df["salario"].median(), inplace=True)
```

 - Categóricos/Textos: valor fixo ou moda
   
```
# Preencher com valor fixo

df["cidade"].fillna("Desconhecida", inplace=True)

# Preencher com a moda (valor mais frequente)

df["categoria"].fillna(df["categoria"].mode()[0], inplace=True)
```

3️⃣ Preencher com regras específicas

 - Quando faz sentido preencher de acordo com outra variável.
   
```
df["idade"] = df.groupby("cidade")["idade"].transform(lambda x: x.fillna(x.mean()))
```

💡 Dicas práticas:

- Para dados numéricos: use média ou mediana.

- Para textos/categorias: use "Desconhecido" ou a moda.

- Sempre analise o impacto da decisão — remover demais pode eliminar padrões importantes.

- A mediana é mais resistente a valores extremos (outliers).
