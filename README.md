plt.figure(figsize=(10, 6))
plt.title('Comparativo de Preços: Alemanha, México e Coreia do Sul', fontdict={'fontweight':'bold', 'fontsize': 14})

# Plotando os novos países
# Lembre-se: usamos o nome da coluna em inglês para o código encontrar os dados
plt.plot(df.Year, df.Germany, 'r.-', label='Alemanha')
plt.plot(df.Year, df.Mexico, 'g.-', label='México')
plt.plot(df.Year, df['South Korea'], 'b.-', label='Coreia do Sul') # Usamos aspas porque tem espaço no nome

plt.xlabel('Ano')
plt.ylabel('Preço (USD)')
plt.legend()
plt.grid(True)

plt.show()
