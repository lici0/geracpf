# Gerador de CPF

Este reposit�rio cont�m a estrutura b�sica do site http://geracpf.com, um micro site que desenvolvi.

## Como funciona?

O site [Gerador de CPF](http://geracpf.com) � voltado para auxiliar deselvovedores que precisam implementar ou testar em seus sistemas a funcionalidade de valida��o de n�meros de CPF (cadastro de pessoas f�sicas), de acordo com a regra dos d�gitos verificadores.

Para gerar um n�mero de CPF v�lido (segundo essa regra) basta acessar o site e clicar no bot�o "Gerar Novo CPF". O resultado ser� exibido no caixa de texto e poder� ser facilmente copiado para uso.

Os d�gitos verificadores s�o calculados atrav�s de um algoritmo que soma o produto de cada d�gito que comp�e o CPF por um peso e calcula o resto da divis�o dessa soma por 11. O c�digo fonte deste algoritmo escrito em JavaScript pode ser obtido [aqui](https://github.com/tome-vilela/geracpf/blob/master/jss/all.js).

Neste c�digo fonte s�o definidas duas fun��es, uma para gerar um n�mero de CPF e outra para valid�-lo:

```
var n = new CPF().generate();

if (new CPF().validate(n)) {
  alert('sucesso!');
}
```

Para quebrar um pouco a monotonia natural de sites voltados � programadores, o [Gerador de CPF](http://geracpf.com) utiliza um layout limpo e direto, com uma imagem de fundo que busca cobrir toda a tela e passar uma sensa��o de tranquilidade:

![http://imgur.com/aJDZVw9](http://i.imgur.com/aJDZVw9.png)

Apesar de ser compat�vel com dispositivos mobile, este site � voltado principalmente para acesso por desktops e notebooks, dado que dificilmente um desenvolvedor ir� codificar atrav�s de um smartphone.

Esperamos que nosso site seja �til a voc�s!

### Contato

Fique � vontade para entrar em contato atrav�s do e-mail tome.vilela@gmail.com