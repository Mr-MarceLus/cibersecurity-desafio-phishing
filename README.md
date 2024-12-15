# Phishing para captura de senhas do Facebook

### Ferramentas

- Kali Linux
- kit de ferramentas de configuração

### Configurando o Phishing no Kali Linux

Acesso root: ``` sudo -i ```

![image](https://github.com/user-attachments/assets/b12ad70d-690d-4b13-9a36-86d23c212275)
  
 Iniciando o setoolkit: ``` setoolkit ```

 ![image](https://github.com/user-attachments/assets/c8d5d608-87b1-4c29-8077-ba244e7a3175)
 
Tipo de ataque: ``` (1) Social-Engineering Attacks ```
 
![image](https://github.com/user-attachments/assets/efeeea3b-c9fa-4186-896c-09d7456857a2)


 
 Vetor de ataque: ``` (2) Web Site Attack Vectors  ```
 
 ![image](https://github.com/user-attachments/assets/1492b6ac-b0e0-4bac-af2e-8e58b929fb4d)

 Método de ataque: ```(3) Credential Harvester Attack Method ```
 
 ![image](https://github.com/user-attachments/assets/64f667e2-d7fc-436d-a868-da21267fba71)

 
 Método de ataque: ``` (2) Site Cloner ```

 ![image](https://github.com/user-attachments/assets/a77d8705-637e-442f-86c5-82cce119cf2c)

  Obtendo o endereço da máquina: ``` ifconfig ```

 ![image](https://github.com/user-attachments/assets/77b8b622-a06b-45f7-af3b-ae1a04ce505c)


 URL para clonar: http://www.facebook.com


### Resutados (Versão sem Defesa)
![image](https://github.com/user-attachments/assets/ecae27ef-b3d3-400a-88c7-ceecfd4d9d6c)

### Defesa Facebook

Atualmente o site do Facebook possui uma proteção contra scripts maliciosos e a resolução proposta não funciona perfeitamente.

![ERRO MÉTODO INICIAL](https://github.com/user-attachments/assets/8d8a8455-dee2-45ed-b8ff-76fae88b142e)


### Alternativa contra a defesa

Isso pode ser contornado no próprio  ```setoolkit``` onde se pode realizar ```Custon Import```. Nesta opção realizaremos uma clonagem e em seguida uma pequena edição no código fonte original. 

![IMPORTAÇÃO PERSONALIZADA](https://github.com/user-attachments/assets/604cae8e-111e-43c3-a530-252871c19bc6)

### Salvar página e botão ID

Na página original, salvaremos a página com o nome ```index.html``` e em seguida funcionaremos o botão ```Log In```. 

![TEMPORIZE O BOTÃO DE IDENTIFICAÇÃO DA PÁGINA](https://github.com/user-attachments/assets/9f8e1356-3777-45eb-9cad-2321909af532)

Em seguida iremos identificar o ID do botão. 

![Botão Identificando ID](https://github.com/user-attachments/assets/ff090128-63be-4c71-ad11-42f34120e83c)

### Editando código fonte

Em seguida iremos copiar o código fonte do site 'www.facebook.com' e colar no nosso arquivo ```index.html```

![COPIANDO COD FONTE DA PÁGINA ORIGINAL](https://github.com/user-attachments/assets/d74c3cba-c485-42a7-9376-fd83dc89e53d)

Agora no código fonte iremos identificar em qual script o ```button ID``` está sendo chamado e em seguida desligar.

![Excluindo script](https://github.com/user-attachments/assets/c8738d9c-cbff-4086-8a5d-a154d369affd)

Em seguida no ```setoolkit``` selecionaremos a opção ```Custom Import``` e apontaremos para a pasta onde o código fonte manipulado se encontrar.

Copie o diretório da pasta onde se localiza o código fonte manipulado.

Cole o diretório no setoolkit. 

![COLAR O DIRETÓRIO](https://github.com/user-attachments/assets/4f49c8a4-9877-4af6-b537-b3ca57533681)

Selecione ```Copiar a pasta inteira```

![OPÇÃO COPIAR A PASTA INTEIRA](https://github.com/user-attachments/assets/7ecadd9c-1229-4e74-9894-f423d6023aa3)

Em seguida defina a ```URL``` do site importado.

![DEFINIR COM A URL DA PÁGINA FONTE](https://github.com/user-attachments/assets/50e80c13-6ea2-42e9-ab2c-399edf6f20dd)

## Resultado após aplicação do método contra a defesa

![USUÁRIO E SENHA](https://github.com/user-attachments/assets/11b8a323-1403-41d8-81d6-1744a0e448be)


