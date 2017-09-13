# Estudo dos casos V e VI

[Caso Imóvel](https://github.com/tmenegaz/db_dendezeiros/blob/master/assunto/casos.md#imóvel "Caso Imóvel")

**Entidades identificadas**  
Vendedor = [-id + nome + cpf + num_creci] -> responsável pela negociata  
Imóvel = [-id + endereco + area_uso + area_tot + dims + bairro + cidade + estado] -> item da negociata  
Anúncio = [-id, prc_min + prc_max + num_oferta + data_0] -> método da negociata  
Comprador = [-id + nome + endereco + cpf + telefone + email] -> alvo da negociata  
Lance_min = [-id, prc_min + data_lance] -> valor minimo de avanço da negociata  

![Relação das Entidades](https://github.com/jota-lucas/databases_senai_dend/blob/master/er1.png "Relacionamento: Entidades do Caso V")

Cada imóvel pode ser anunciado em um ou mais anuncios  
Cada anúncio deve ser administrado por um vendedor/agente  
Cada comprador pode dar lance em um ou mais anuncios  
Cada vendedor pode administrar um ou mais anuncios  

[Caso Cadastro de Pessoa](https://github.com/tmenegaz/db_dendezeiros/blob/master/assunto/casos.md#cadastro-de-pessoa "Caso Cadastro de Pessoa")

**Entidades identificadas**  
Cliente Físico = [-id + nome + sobrenome + telefone + endereco + data de nasc + cpf + email] -> alvo do formulario  
Cliente Jurídico = [-id + nome_emp + telefone + endereco + cnpj + email] -> alvo do formulario  
Fábrica = [-id + nome_fab + telefone + endereco + cnpj + email] -> gerador do formulario  
Produto = [-id + nome + preco] -> motivo do formulario

![Relação das Entidades](https://github.com/jota-lucas/databases_senai_dend/blob/master/er2 "Relacionamento: Entidades do Caso VI")

Cada cliente físico deve preencher o formulario a fim de adquirir os produtos da fabrica  
Cada cliente jurídico deve preencher o formulario a fim de adquirir os produtos da fabrica  
