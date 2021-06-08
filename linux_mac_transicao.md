# Migração de usuários de Ubuntu para MacOS
## Teclado externo
Por padrão as teclas de modificação são mapeadas desta forma:
  * control	- Ctrl
  * option	- Alt
  * command	- Winkey/Super
  * shift	- Shift

## Atalhos úteis
### Uso do sistema
  * **control + A**	- função da tecla HOME no Windows e Linux, retorna para o início da linha
  * **control + E** 	- função da tecla END no Windows e Linux, vai para o fim da linha
  * **control + UP** *(seta para cima)*	- Mission Control - mostra todas as janelas abertas em formato de mosaico
  * **control + DOWN** *(seta para baixo)*	- mostra todas as janelas da aplicação atual
  * **control + LEFT/RIGHT** *(setas esquerda e direita)*	- transita entre áreas de trabalho
  * **command + SPACE** *(barra de espaço)*	- **Spotlight** (inicializador de aplicações)
### Finder
  * **command + UP** *(seta para cima)*	- subir um diretório

## Alterar timeout do comando sudo (acredito que o Device Enrollment reseta esse dado, visto que meu terminal perdeu o timeout)
Por padrão o timeout leva 5 minutos no linux, no MacOs, no entanto, o padrão é não haver timeout. Para mudar esse comportamento siga os passos abaixo.

No terminal use o comando abaixo (importante usar o vi para editar o arquivo):

```
sudo visudo
```

Dentro do arquivo altere a linha

```
Defaults timestamp_timeout=0 (trocar o 0 por x minutos)
```

### Para não-usuários de Vi/Vim:
#### Find
Para procurar dentro do arquivo, certifique-se estar no modo NORMAL (nada escrito no rodapé da janela, caso haja as palavras VISUAL ou INSERT, pressione ESC), digite:

```
/(sua_pesquisa)
```

E pressione enter, em seguida use n para ir à próxima ocorrência ou N (dessa vez maiúsculo) para a ocorrência anterior

#### Salvar
Dentro do modo normal (nada escrito no rodapé da janela, caso haja as palavras VISUAL ou INSERT, pressione ESC)
* :wq	-	salvar as alterações e fechar o arquivo
* :q	-	fechar um arquivo não modificado
* :q!	-	fechar um arquivo modificado sem salvar

---
Work in progress
