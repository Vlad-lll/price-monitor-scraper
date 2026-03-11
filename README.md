# 🛒 Monitor de Preços - Web Scraper (Bypass Cloudflare)

Um script em Python desenvolvido para monitorar preços de hardwares e periféricos em e-commerces (como a KaBuM!), extraindo dados diretamente do HTML da página. O diferencial deste projeto é a utilização de técnicas para contornar proteções antibot (como o Cloudflare) e a limpeza de strings para conversão de moedas em valores decimais (Float).

## 🚀 Funcionalidades

- **Bypass de Segurança:** Utiliza a biblioteca `cloudscraper` para simular requisições de um navegador real (Google Chrome no Windows), evitando bloqueios de scraping.
- **Extração Precisa (Parsing):** Navega pela árvore DOM do site com `BeautifulSoup4` para isolar a tag exata contendo o preço atualizado.
- **Tratamento de Dados:** Limpa os dados brutos extraídos do HTML (removendo símbolos como "R$", espaços invisíveis `&nbsp;` e `\xa0`) e converte as strings para o formato numérico (`float`) do Python, permitindo futuras operações matemáticas e lógicas.

## 🛠️ Tecnologias Utilizadas

- **[Python 3.x](https://www.python.org/)** - Linguagem principal do projeto.
- **[BeautifulSoup4](https://pypi.org/project/beautifulsoup4/)** - Para extração e manipulação dos dados HTML.
- **[Cloudscraper](https://pypi.org/project/cloudscraper/)** - Para contornar os desafios de segurança (Cloudflare) da loja.

## ⚙️ Como executar o projeto

### Pré-requisitos
É necessário ter o [Python](https://www.python.org/downloads/) instalado em sua máquina.

### Passo a passo

1. Clone este repositório:
   ```bash
   git clone [https://github.com/SEU-USUARIO/monitor-de-precos.git](https://github.com/SEU-USUARIO/monitor-de-precos.git)
