- 👋 Hi, I’m @EricaZamproni39
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
EricaZamproni39/EricaZamproni39 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
ef decodificar_texto(texto):
    resultado = ""
    for char in texto:
        if char.isalpha():
            # Verifica se o caractere é uma letra
            proximo_char = chr((ord(char) - 96) % 26 + 97) if char.islower() else chr((ord(char) - 64) % 26 + 65)
            resultado += proximo_char
        else:
            # Mantém o caractere inalterado se não for uma letra
            resultado += char
    return resultado

# Exemplo de uso
texto_codificado = "Olá, Mundo!"
texto_decodificado = decodificar_texto(texto_codificado)
print("Texto original:", texto_codificado)
print("Texto decodificado:", texto_decodificado)
