#Antes de tudo, faça a instalação da biblioteca abaixo separadamente.
pip install pillow

#Após a instalação, pode continuar.
from PIL import Image
import os

def converter_para_webp(pasta_origem, pasta_destino):
    if not os.path.exists(pasta_destino):
        os.makedirs(pasta_destino)

    arquivos = os.listdir(pasta_origem)

    for arquivo in arquivos:
        caminho_origem = os.path.join(pasta_origem, arquivo)
        caminho_destino = os.path.join(pasta_destino, os.path.splitext(arquivo)[0] + ".webp")

        
        imagem = Image.open(caminho_origem)

        # Salvar a imagem no formato WebP
        imagem.save(caminho_destino, "WEBP")

#COLOCAR AQUI OS ENDEREÇOS DAS PASTAS DE ORIGEM E DESTINO
#Importante manter as "\\" duplas.

if __name__ == "__main__":
    pasta_origem = "C:\\Users\\seu_user\\Downloads\\pastaX"
    pasta_destino = "C:\\Users\\seu_user\\Downloads\\pastaY"

    converter_para_webp(pasta_origem, pasta_destino)
