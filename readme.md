O arquivo que gera o conteúdo da página tem duas partes. Na primeira você coloca os seus dados e links de contato. Na segunda parte os conteúdos publicados. Até o momento estamos aceitando conteúdos no formato de link (para uma outra página web), Instagram e Youtube. Quando der um tempinho vamos colocar Facebook também.

## Primeira parte 
### Formato do arquivo
| Campo | Descrição |
|--- | --- |
| layout: | Hoje temos somente a opção **participantes**. |
| nome: | Escreva o seu nome. Observe se o tamanho se encaixa no layout da página. |
| atividade: | Como você vai aparecer na página? Por exemplo: **Professor**, **Professor de Robótica**, **Coordenador de Tecnologia**, etc. |
| empresa: | Onde você trabalha? Pode ser o nome da escola ou da secretaria de educação do seu estado. Este campo é opcional. |
| foto: | Nome do arquivo com a sua foto. |
| facebook: | Link completo para a sua página no Facebook. Por exemplo: https://www.facebook.com/ACriatividadeDigital/. Este campo é opcional |
| linkedin: | Link completo para a sua página no Facebook. Por exemplo: https://www.linkedin.com/in/parau/ . Este campo é opcional. |
| instagram: | Nome do usuário no Instragram. Escreva sem o **@**. Por exemplo: **parau.branco**. Este campo é opcional. |
| site: | Endereço do seu site ou do site da sua escola. Escrever sem o https. Por exemplo: tecnologia.educacional.com.br. Este campo é opcional. |
| cidade: | Cidade que você representa. |
| bio: | Breve resumo. Não usar quebra de linha, ou seja, todo o texto no mesmo parágrafo. |

### Exemplo de um arquivo
    ---
    layout: participantes
    nome: Parau Branco
    atividade: Professor
    empresa: CRIATIVIDADE.digital
    foto: paraubranco.jpg
    facebook: https://www.facebook.com/ACriatividadeDigital/
    linkedin: https://www.linkedin.com/in/parau/
    instagram: parau.branco
    site: criatividade.digital
    cidade: Curitiba
    bio: Parahuari é apaixonado pela área de educação. Ele tem mais de 20 anos de experiência no desenvolvimento de soluções tecnológicas voltadas a aprendizagem. Ao longo desses anos, Parahuari teve a oportunidade de desempenhar diferentes papéis como professor, programador, autor, designer instrucional, gerente de projetos e pesquisador. Parau, como também é chamado, trabalhou no desenvolvimento de diferentes tipos de soluções educativas como portais educacionais, livros didáticos digitais, simulações, sistemas adaptativos e jogos educativos. Agora ele está envolvido na pesquisa e desenvolvimento de soluções que incentivam a leitura e promovem a criatividade digital. Parahuari acredita que melhorar a educação é também melhorar o mundo.
    ---

## Segunda parte
### Formato do arquivo
| Campo | Descrição |
| --- | --- |
| conteudos: | Indicação de que a seguir serão listados os conteúdos. Não precisa preencher nada nesta linha. |
| - topico: | Nome do tópico de conteúdo. Na página é o texto que aparece com fonte maior e na cor verde. |
|   itens: | Itens de conteúdo que farão parte deste tópico. Não precisa preencher nada nesta linha. |
|     - tipo: | Tipo de conteúdo. Pode ser **link**, **youtube** ou **instagram**. |
|       descricao: | Texto que vai ser apresentado antes do conteúdo. Não usar quebra de linha, ou seja, todo o texto no mesmo parágrafo. Se precisar quebrar a linha use a marca a tag HTML **&lt;br&gt;**.|
|       link: | Endereço (URL) para acesso ao conteúdo. Usar este campo apenas quando o tipo de conteúdo for link. |
|       largura: | Campo só para os conteúdos do tipo **youtube** e **instagram**. Indica a largura do vídeo publicado. |
|       altura: | Mesmo do **largura** mas com a altura do vídeo publicado. |
|       id: | Código do vídeo publicado no **youtube** ou **instagram**. Você encontra ele no link de compartilhamento. Veja os exemplos (negrito): youtu.be/**OrpdJCSuXrU** ou instagram.com/tv/**CBbLNEYACQt**/. |

### Exemplo de um arquivo
    conteudos:
      - topico: Conhecendo o SPIKE Prime
        itens: 
        - tipo: instagram
          descricao: Unboxing do lançamento mundial da LEGO, o SPIKE Prime!!
          largura: 582
          altura: 1035
          id: CBbLNEYACQt
      - topico: Dicas sobre o uso do SPIKE Prime
        itens: 
          - tipo: link
            descricao: Montei este site com dicas sobre o funcionamento do LEGO® Education SPIKE™ Prime. Se tiver alguma dúvida ou quiser contribuir com este texto, deixe seu comentário no site.
            link: https://lego.criatividade.digital/dicas
      - topico: Passo a passo com recurso 3D
        itens: 
          - tipo: link
            descricao: Desenvolvi este experimento de passo a passo 3D. Usei como base neste trabalho o Studio para modelagem e código de visualização web usado no ldraw.org.
            link: https://lego.criatividade.digital/r/0007/new/passo-a-passo.htm
      - topico: Brincando com os sensores de Distância e Cores
        itens: 
          - tipo: youtube
            descricao: Uma brincadeira usando a programação dos sensores de CORES e DISTÂNCIA. Também foram programados a matriz de leds e a luz do botão central. <b>Teatro</b> + <b>LEGO</b> 😀
            largura: 560
            altura: 315
            id: OrpdJCSuXrU
      - topico: Desafio usando o sensor giroscópio
        itens: 
          - tipo: youtube
            descricao: Aproveitando o tópico giroscópio trabalhado pelos <i>influencers</i> experimentei programar um <i>self balancing robot</i>. Experimentei com o Hub em duas posições. E, no vídeo, transformando a brincadeira em um grande circo. 😜
            largura: 560
            altura: 315
            id: GvrpnCbgDfo

## Primeira + Segunda parte
Bem... Para concluir o trabalho basta junta a primeira com a segunda parte. 😜 Veja abaixo. Outros exemplos você encontra aqui no Github. Veja os arquivos com extensão **.md** disponíveis neste repositório! 👆👆 😀

    ---
    layout: participantes
    nome: Parau Branco
    atividade: Professor
    empresa: CRIATIVIDADE.digital
    foto: paraubranco.jpg
    facebook: https://www.facebook.com/ACriatividadeDigital/
    linkedin: https://www.linkedin.com/in/parau/
    instagram: parau.branco
    site: criatividade.digital
    cidade: Curitiba
    bio: Parahuari é apaixonado pela área de educação. Ele tem mais de 20 anos de experiência no desenvolvimento de soluções tecnológicas voltadas a aprendizagem. Ao longo desses anos, Parahuari teve a oportunidade de desempenhar diferentes papéis como professor, programador, autor, designer instrucional, gerente de projetos e pesquisador. Parau, como também é chamado, trabalhou no desenvolvimento de diferentes tipos de soluções educativas como portais educacionais, livros didáticos digitais, simulações, sistemas adaptativos e jogos educativos. Agora ele está envolvido na pesquisa e desenvolvimento de soluções que incentivam a leitura e promovem a criatividade digital. Parahuari acredita que melhorar a educação é também melhorar o mundo.
    conteudos:
      - topico: Conhecendo o SPIKE Prime
        itens: 
        - tipo: instagram
          descricao: Unboxing do lançamento mundial da LEGO, o SPIKE Prime!!
          largura: 582
          altura: 1035
          id: CBbLNEYACQt
      - topico: Dicas sobre o uso do SPIKE Prime
        itens: 
          - tipo: link
            descricao: Montei este site com dicas sobre o funcionamento do LEGO® Education SPIKE™ Prime. Se tiver alguma dúvida ou quiser contribuir com este texto, deixe seu comentário no site.
            link: https://lego.criatividade.digital/dicas
      - topico: Passo a passo com recurso 3D
        itens: 
          - tipo: link
            descricao: Desenvolvi este experimento de passo a passo 3D. Usei como base neste trabalho o Studio para modelagem e código de visualização web usado no ldraw.org.
            link: https://lego.criatividade.digital/r/0007/new/passo-a-passo.htm
      - topico: Brincando com os sensores de Distância e Cores
        itens: 
          - tipo: youtube
            descricao: Uma brincadeira usando a programação dos sensores de CORES e DISTÂNCIA. Também foram programados a matriz de leds e a luz do botão central. <b>Teatro</b> + <b>LEGO</b> 😀
            largura: 560
            altura: 315
            id: OrpdJCSuXrU
      - topico: Desafio usando o sensor giroscópio
        itens: 
          - tipo: youtube
            descricao: Aproveitando o tópico giroscópio trabalhado pelos <i>influencers</i> experimentei programar um <i>self balancing robot</i>. Experimentei com o Hub em duas posições. E, no vídeo, transformando a brincadeira em um grande circo. 😜
            largura: 560
            altura: 315
            id: GvrpnCbgDfo
    ---