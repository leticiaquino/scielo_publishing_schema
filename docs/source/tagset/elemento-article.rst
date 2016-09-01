.. _elemento-article:

<article>
=========

Aparece em:

  ``/``

Atributos obrigatórios:

  1. ``@dtd-version``
  2. ``@article-type``
  3. ``@xml:lang``
  4. ``@xmlns:xlink="http://www.w3.org/1999/xlink"``
  5. ``@specific-use="sps-1.0"``

.. note:: No atributo ``@specific-use`` o valor **sps-1.0** é apenas uma referência genérica à versão da *SciELO PS*. Deve ser utilizada sempre          a versão corrente (atual).

Ocorre:

  Uma vez


:ref:`elemento-article` é a raiz do *XML* do :term:`documento` e deve explicitar, obrigatoriamente, os atributos de versão da :term:`DTD`, tipo de documento, idioma do texto, declarações de :term:`namespace` e versão da :term:`SciELO PS` utilizada.

O atributo ``@xmlns:mml="http://www.w3.org/1998/Math/MathML"`` é opcional e deve ser utilizado sempre que equações do tipo :term:`MathML` forem identificadas no :term:`documento`.

Para ``@dtd-version`` deve-se utilizar o valor 1.0 conforme a :term:`DTD`, explicitada em :ref:`xml-doctype`.

Para tipo de documento (``@article-type``) os valores possíveis são:

+--------------------+----------------------------------------------------------+
| Valor              | Descrição                                                |
+====================+==========================================================+
|                    | Comentários - Nota crítica ou esclarecedora, escrita     |
|                    | para discutir, apoiar ou debater um artigo ou outra      |
| article-commentary | apresentação publicada anteriormente.                    |
|                    | Pode ser um artigo, carta, editorial, etc. Estas         |
|                    | publicações podem aparecer como comentário, comentário   |
|                    | editorial, ponto de vista, etc.                          |
+--------------------+----------------------------------------------------------+
|                    | Resenha - Análise crítica de livros e outras             |
| book-review        | monografias.                                             |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Comunicação breve - Informe sucinto acerca de            |
| brief-report       | resultados de uma pesquisa.                              |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Relato, descrição ou estudo de caso - Pesquisas          |
| case-report        | especiais que despertam interesse informativo.           |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Errata - Corrige erros apresentados em artigos após sua  |
| correction         | publicação online e/ou impressa.                         |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Editorial - Uma declaração de opiniões, crenças e        |
|                    | políticas do editor do periódico, geralmente sobre       |
| editorial          | assuntos de interesse da comunidade científica e da      |
|                    | sociedade.                                               |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Press release - Comunicação breve de linguagem           |
| in-brief           | jornalística sobre um artigo ou tema.                    |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Cartas - Correspondência escrita entre pessoas ou        |
| letter             | instituições, geralmente comentando um trabalho          |
|                    | publicado.                                               |
+--------------------+----------------------------------------------------------+
|                    | Outro tipo de documento - Pode ser considerado adendo,   |
| other              | anexo, discussão, artigo de preocupação, introdução      |
|                    | entre outros.                                            |
+--------------------+----------------------------------------------------------+
| partial-retraction | Retratação ou recusa de parte de materiais já publicados |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Comunicação breve - Informe sobre atualização de         |
| rapid-communication| investigação ou outra notícia.                           |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Resposta (a carta ou comentário) - Geralmente é usado    |
| reply              | pelo autor original e contém comentários adicionais a    |
|                    | outros anteriormente escritos.                           |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Artigo original - Abrange pesquisas, experiências        |
| research-article   | clínicas ou cirúrgicas e/ou outras contribuições         |
|                    | originais.                                               |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Retratação (de um artigo científico) - Instrumento para  |
| retraction         | corrigir um registro acadêmico publicado equivocadamente,|
|                    | por plágio, por exemplo.                                 |
+--------------------+----------------------------------------------------------+
|                    | Revisões de literatura - Avaliações críticas             |
| review-article     | sistematizadas da literatura sobre determinado assunto.  |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Tradução - Artigo traduzido a partir de original escrito |
| translation        | em outro idioma.                                         |
|                    |                                                          |
+--------------------+----------------------------------------------------------+


.. note:: O atributo tipo de documento não deve ser confundido com a seção em que o :term:`documento` aparece no sumário.


O idioma do texto (``@xml:lang``) é descrito pela norma :term:`ISO 639-1` como um código de dois caracteres alfabéticos em caixa baixa, cujo conteúdo encontra-se disponível no `site <http://www.mathguide.de/info/tools/languagecode.html>`_.

O atributo ``@specific-use`` identifica a versão utilizada da :term:`SciELO Publishing Schema`.

Exemplo (tag completa da `JATS versão 1.0 <http://jats.nlm.nih.gov/publishing/1.0/>`_):

.. code-block:: xml

     <article xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:mml="http://www.w3.org/1998/Math/MathML" dtd-version="1.0" specific-use="sps-1.0" article-type="research-article" xml:lang="en">

           ...

	 </article>


.. {"reviewed_on": "20160728", "by": "gandhalf_thewhite@hotmail.com"}
