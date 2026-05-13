# MoodCoffee Bot
Meu primeiro chat bot

#funcionalidade Um chatbot que conversa com a pessoa baseado no humor dela e recomenda:

cafés;
músicas;
frases;
filmes;
comidas;
atividades;
playlists.

A ideia é parecer um “barista virtual emocional”.

#Exemplo de conversa 

Usuário:
Estou cansado hoje.

Bot:
Você precisa de algo leve ☕
Recomendação:
- Cappuccino
- Playlist lo-fi
- Filme: A Vida Secreta de Walter Mitty

#Funcionalidades 
- Detectar humor por palavras-chave
- Recomendar cafés
- Recomendar músicas
- Frases motivacionais
- Sugestões de filmes

# Codigo
# app.py

print("☕ MoodCoffee Bot iniciado!")
print("Digite 'sair' para encerrar.\n")

while True:
    mood = input("Como você está se sentindo hoje? ").lower()

    if mood == "sair":
        print("Até mais ☕")
        break

    elif "cansado" in mood:
        print("""
☕ Recomendação do MoodCoffee Bot

Café: Cappuccino
Música: Playlist Lo-fi
Filme: A Vida Secreta de Walter Mitty
Dica: Tire alguns minutos para descansar.
""")

    elif "feliz" in mood or "animado" in mood:
        print("""
⚡ Energia alta detectada!

Café: Espresso duplo
Música: Indie Rock
Atividade: Caminhada ao ar livre
Frase: Continue aproveitando esse momento!
""")

    elif "triste" in mood:
        print("""
💙 Parece que você precisa relaxar.

Café: Chocolate quente
Filme: Soul
Música: Piano Relaxante
Frase: Dias difíceis também passam.
""")

    elif "estressado" in mood:
        print("""
🌿 Hora de desacelerar.

Bebida: Chá de camomila
Música: Jazz suave
Atividade: Respiração profunda
Dica: Faça uma pausa de 5 minutos.
""")

    else:
        print("""
🤔 Não consegui identificar seu humor.

Tente usar palavras como:
- cansado
- feliz
- triste
- estressado
""")


