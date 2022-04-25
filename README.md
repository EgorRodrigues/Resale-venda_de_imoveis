## Prova Técnica - Pessoa Desenvolvedora 
### Contexto 

A Resale é uma startup brasileira de tecnologia para a área imobiliária. Com crescimento significativo a cada ano, a Resale vem sendo destaque na mídia especializada. No ano de 2021 a empresa está passando por um grande crescimento, tanto em número de funcionários como em portfólio de produtos. Em termos de tecnologia, trabalhamos com o que há de mais moderno em infraestrutura baseada nos produtos da Amazon AWS. 

### Objetivo 
Atualmente, as funcionalidades mais básicas da nossa plataforma envolvem registro e disponibilização do imóvel para venda para nossos clientes. Entretanto, esse fluxo contém algumas regras que precisam ser atendidas. 
O objetivo dessa prova é desenvolver uma pequena plataforma de registro e venda de imóveis. Deverão ser respeitadas as regras que estão anotadas neste documento. 

## Entidades 

### Imóvel: 
- Nome* 
- Endereço*
- Descrição 
- Status: Ativo ou Inativo* 
- Características (Número de quartos, salas, banheiros, vagas de garagem, etc...)* 
- Tipo (Apartamento, Casa, Prédio etc)* 
- Finalidade (Residencial, Escritório, Comercial, etc)* 
- Valor avaliado* 
  - Valor avaliado do imóvel frente ao mercado 
- Valor do imóvel* 
  - Valor do imóvel para a venda

### Carteira de imóveis: 
- Nome* 
- Tipo de venda: Venda direta, Imobiliária ou Leilão* 
- Taxa de comissão (%)* 
- Canal de venda* 
  Canal de venda: 
- Nome* 
- Tipo de canal de venda: Venda direta, Imobiliária ou Leiloeiro* Obs: *campos obrigatórios 

### Regras de negócio: 
#### Imóvel: 

- Valor total do imóvel: Valor do imóvel somado ao valor da comissão da carteira ● Deságio do valor do imóvel: O desconto do imóvel em relação ao valor avaliado ● Caso o imóvel não esteja ativo, ele não deverá retornar na Listagem "portal" 
  Relação Imóvel x Carteira: 
- O imóvel pode estar em somente 1(uma) carteira de venda direta e N de imobiliária. ● O imóvel pode estar em N carteiras de imobiliária. 
- O imóvel pode estar somente em 1 carteira de leilão. 

#### Relação Carteira x Canal de venda: 
- O canal de venda só pode estar dentro da carteira que corresponde ao seu tipo:
  - ex: Canal de Venda direta só pode ser relacionado a carteira do tipo Venda Direta 

#### Funcionalidades: 
- CRUD de imóvel 
- CRUD de carteira de imóveis 
- CRUD de canal de venda 
- Relacionamento imóvel com carteira de imóveis 
- Listagem "portal"
  - É a listagem que disponibiliza ao cliente as informações básicas para venda do imóvel 
    - Refer: PORTAL RESALE 
  - Informações: 
      - Nome do imóvel 
      - Endereço do imóvel 
      - Descrição do imóvel
      - Características do imóvel 
      - Tipo do imóvel 
      - Finalidade do imóvel 
      - Valor total do imóvel 
      - Deságio do valor do imóvel 
      - Tipo de venda da carteira 
      - Nome do canal de venda 
### Requisitos: 
      
- A solução pode ser desenvolvida em qualquer linguagem de programação e banco de dados
- Documentação

### Pontos avaliados: 
- Funcionamento da API 
- Arquitetura de software 
- Qualidade de documentação 
- Organização 
- Testes

### Diferencial 
- Python 
- Mysql 
- Docker 
- Alguma ferramenta de CD ex: Heroku 

### Entrega: 
      Prazo: 7 dias contados a partir da data do recebimento do teste. 
      Envio do código: O código deverá ser publicado em um repositório GIT privado e compartilhado com o e-mail do desenvolvedor que será enviado juntamente com a prova. 
      
### BOA SORTE!
