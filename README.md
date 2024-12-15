# Phishing para captura de senhas do Facebook

### Ferramentas

- Kali Linux
- kit de ferramentas de configuração

### Configurando o Phishing no Kali Linux

- Acesso root: ``` sudo -i ```
![image](https://github.com/user-attachments/assets/b12ad70d-690d-4b13-9a36-86d23c212275)

- 
- Iniciando o setoolkit: ``` setoolkit ```
- Tipo de ataque: ``` (1)Ataques de Engenharia Social ```
- Vetor de ataque: ``` (2)Vetores de ataque a sites ```
- Método de ataque: ```(3)Credential Harvester Attack Method ```
- Método de ataque: ``` (2)Site Cloner ```
- Obtendo o endereço da máquina: ``` ifconfig ```
- URL para clonar: http://www.facebook.com

### Resultados
### Resutados (Versão sem Defesa)
![Texto alternativo](./passwd.png "Título opcional")
### Defesa Facebook
->Observe abaixo que atualmente o site do Facebook possui uma proteção contra scripts maliciosos. 
![ERRO MÉTODO INICIAL](https://github.com/user-attachments/assets/8d8a8455-dee2-45ed-b8ff-76fae88b142e)
### Alternativa contra a defesa
->Uma possibilidade de resolução do caso, não é o próprio ```setoolkit``` onde se pode realizar ```Custon Import```. Nesta opção realizaremos uma clonagem e em seguida uma pequena edição no código fonte original. 
![IMPORTAÇÃO PERSONALIZADA](https://github.com/user-attachments/assets/604cae8e-111e-43c3-a530-252871c19bc6)
### Salvar página e botão ID
->Na página original, salvaremos a página com o nome ```index.html``` e em seguida funcionaremos o botão ```Log In```. 
![TEMPORIZE O BOTÃO DE IDENTIFICAÇÃO DA PÁGINA](https://github.com/user-attachments/assets/9f8e1356-3777-45eb-9cad-2321909af532)
->Em seguida iremos identificar o ID do botão. 
![Botão Identificando ID](https://github.com/user-attachments/assets/ff090128-63be-4c71-ad11-42f34120e83c)
### Editando código fonte
->Em seguida iremos copiar o código fonte do site 'www.facebook.com' e colar no nosso arquivo ```index.html```
![COPIANDO COD FONTE DA PÁGINA ORIGINAL](https://github.com/user-attachments/assets/d74c3cba-c485-42a7-9376-fd83dc89e53d)
->Agora no código fonte iremos identificar em qual script o ```button ID``` está sendo chamado e em seguida desligar.
![Excluindo script](https://github.com/user-attachments/assets/c8738d9c-cbff-4086-8a5d-a154d369affd)
->Em seguida no ```setoolkit``` selecionaremos a opção ```Custom Import``` e apontaremos para a pasta onde o código fonte manipulado se encontrar.
->Copie o diretorino da pasta onde se localiza o código fonte manipulado.
->Cole o diretório no setoolkit. 
![COLAR O DIRETÓRIO](https://github.com/user-attachments/assets/4f49c8a4-9877-4af6-b537-b3ca57533681)
->Selecione ```Copiar a pasta inteira```
![OPÇÃO COPIAR A PASTA INTEIRA](https://github.com/user-attachments/assets/7ecadd9c-1229-4e74-9894-f423d6023aa3)
->Em seguida defina a ```URL``` do site importado.
![DEFINIR COM A URL DA PÁGINA FONTE](https://github.com/user-attachments/assets/50e80c13-6ea2-42e9-ab2c-399edf6f20dd)
## Resultado após aplicação do método contra a defesa
![USUÁRIO E SENHA](https://github.com/user-attachments/assets/11b8a323-1403-41d8-81d6-1744a0e448be)


