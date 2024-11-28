Project created to study chatbot behavior

using GPT-4 of OPENAI and language Python

#Import
import openai

# Chave
openai.api_key = "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"

#Função principal do programa em python
def main():

    print("\nBem-vindo ao GPT-4 Chatbot do Projeto 2 teste")
    print("Digite 'sair' a qualquer momento para encerrar o chat)")

    #Loop
    while True:

      #Coleta a pergunta digitada pelo usuário.
      user_message = input("\nVocê:")

      #Se a mensagem for 'sair' finaliza o programa.
      if user_message.lower() == "sair":
          break

      #Coloca a mensagem digitada pelo usuário na variável Python.
      gpt4_prompt = f"\nUsuário: {user_message}\nChatbot:"

      #Obtém a resposta do modelo executando a função gera_texto()
      chatbot_response = gera_texto(gpt4_prompt)

      #Imprime a resposta do chatbot.
      print(f"\nChatbot: {chatbot_response}")

#Execução do programa (bloco main) em Python
if __name__ == "__main__":
    main()
