# Mini-projeto-ndice-invertido-para-busca-textual
Desenvolvimento de um mecanismo de busca textual utilizando tabelas hash (dicionários), conjuntos e listas.

Pré-requisitos:
Certificar-se de que a versão instalada do Python na sua máquina esteja atualizada . Pode verificar abrindo o terminal e executando:

python --version

Passo 1: Organizar os arquivos do projeto:
Cria uma pasta no computador dedicada a este mini-projeto.
Guardar o código com as funções de busca no arquivo principal chamado indice_invertido.py.
Guardar o script de testes no arquivo chamado experimentos.py.

Passo 2: Preparar o texto para os testes:
Acesse um site de domínio público (como o Project Gutenberg) e baixe a obra Dom Casmurro em formato de texto simples (.txt)
Guarde esse arquivo de texto dentro da mesma pasta dos scripts Python, e os nomei exatamente como texto_teste.txt.

Passo 3: Executar as medições de desempenho:
Abra o terminal e navege até à pasta do seu projeto utilizando o comando cd (exemplo: cd Documentos/mini-projeto-hash).
Execute o arquivo de experimentos com o seguinte comando:

python experimentos.py

O terminal irá processar o arquivo de texto e exibir os tempos (em milissegundos) gastos na varredura completa, na construção do índice e nas 1000 buscas com o índice invertido. Utilize esses valores para preencher as tabelas do seu relatório.

Passo 4 (Opcional): Executar consultas personalizadas:
Se quiseres testar frases ou palavras específicas por conta própria num novo arquivo Python, só precisa importar as funções que você criou e imprimir os resultados:

from indice_invertido import construir_indice, buscar, buscar_e, buscar_ou

texto_simples = "Python é uma linguagem\nEstruturas de dados em Python"
indice = construir_indice(texto_simples)

print(buscar(indice, "python"))
