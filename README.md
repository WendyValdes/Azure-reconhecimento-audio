Conversão de Áudio para Texto – Azure Speech


Descrição

Projeto que converte áudio em texto e texto em áudio usando os serviços Azure Speech (TTS/STT). Suporta arquivos .wav e converte .opus automaticamente.



Funcionalidades

Text-to-Speech (TTS) em português do Brasil

Speech-to-Text (STT) de arquivos de áudio

Conversão automática de .opus para .wav

Upload direto de áudios pelo Colab



Tecnologias

Python | Azure Speech SDK | FFmpeg | Pydub | Google Colab



Como usar

Configure chave e região do Azure no código.

Use TTS para gerar áudio a partir de texto.

Faça upload de arquivos .opus ou .wav.

Execute a conversão automática se necessário.

Use STT para transcrever áudio em texto.



Exemplo rápido

TTS:

speech_synthesizer.speak_text_async("Olá! Teste TTS").get()


STT:

result = speech_recognizer.recognize_once_async().get()
print(result.text)
