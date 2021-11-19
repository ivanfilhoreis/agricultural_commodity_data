# Notícias agrícolas em pt-br

Os datasets presentes nessa pasta contém informações sobre algumas das principais commodities do Brasil. 

 ## Informações gerais
Os dados textuais foram extraídos do site [Notícias Agrícolas](https://www.noticiasagricolas.com.br/), entre esses dados estão, data da notícia, link, manchete, matéria. Dados númericos (preços) foram extraídos do site [Cepea USP](http://www.cepea.esalq.usp.br/br) que fornecem dados sobre o agronegócio no Brasil. 

 ## Informações do notebook utilizado

Com este notebook é possível extrair os dados de todas as categorias de notícias do site ***Notícias Agrícolas***, porém para a criação dos datasets finais é preciso verificar se as séries temporais da categoria desejada está disponível no ***Cepea USP*** para download.

O notebook criado para a automação está disponível em: https://colab.research.google.com/drive/1oosnCTNK6XoSmcKXJm1qeM1ilKuTb3Rm?usp=sharing. 

### Descrição das colunas do dataset

* **date:** data em que a matéria foi publicada. 
* **link:** link para a publicação da matéria. 
* **headline:** manchete da matéria. 
* **text:** texto publicado. 
* **cepea_real:** preço do dia na moeda real fornecido pelo ***Cepea USP***. 
*  **cepea_dollar:** preço do dia na moeda dolar fornecido pelo ***Cepea USP***.
*  **percentage_real:** cálculo representando o aumento/baixa intradia na moeda real. 
*  **percentage_dollar:** cálculo representando o aumento/baixa intradia na moeda dollar.
*  **trend:** a atribuição deste atributo é feita a partir do valor do atributo ***percentage_real***, caso acima de 0.5% é atribuída um valor ***Up***, caso contrário o valor atribuído é ***Down***. 
*  **tarjet:** Para uso em algoritmos de ML, tem o mesmo propósito do atributo ***trend***. Atribuído valor 1 para Up e 0 para Down. 
