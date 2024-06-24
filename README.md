# Projeto de Geração e Leitura de Gabaritos

Este projeto consiste em um script Python para geração e leitura de gabaritos. Ele permite criar uma folha de gabarito em formato A4 com até 180 questões, cada uma com 5 alternativas (A, B, C, D, E), e inclui um QR code identificador. O projeto também oferece uma funcionalidade para ler a imagem de um gabarito preenchido, detectar e reconhecer as alternativas marcadas, e retornar os resultados em um formato JSON.

## Funcionalidades

- **Geração de Gabarito**
  - Gerar uma folha de gabarito em formato A4.
  - Incluir até 180 questões, com 5 alternativas cada.
  - Incluir um QR code identificador na folha.
  - Salvar a folha de gabarito como arquivo (PNG, JPEG, PDF).

- **Leitura de Gabarito**
  - Ler a imagem de um gabarito preenchido.
  - Detectar e reconhecer as alternativas marcadas.
  - Tratar possíveis dificuldades devido a imagens tiradas de celular (ângulos variados, iluminação, etc.).
  - Retornar um dicionário JSON com o número da questão e a alternativa preenchida.

## Instalação

### Pré-requisitos

- Python 3.x
- Virtualenv (opcional, mas recomendado)

### Passos para Instalação

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/projeto-gabarito.git
   cd projeto-gabarito
   ```

2. Crie e ative um ambiente virtual:
   ```bash
   python -m venv venv
   source env/bin/activate  # No Windows, use `venv\Scripts\activate`
   ```

3. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

## Uso

### Geração de Gabarito

Execute o script de geração de gabarito:
```bash
python gerar_gabarito.py
```

### Leitura de Gabarito

Execute o script de leitura de gabarito:
```bash
python ler_gabarito.py caminho/para/imagem-do-gabarito.png
```

## Estrutura do Projeto

```plaintext
projeto-gabarito/
├── README.md
├── requirements.txt
├── gerar_gabarito.py
├── ler_gabarito.py
├── utils/
│   ├── desenho.py
│   ├── qr_code.py
│   ├── leitura.py
│   ├── processamento.py
└── testes/
    ├── test_desenho.py
    ├── test_qr_code.py
    ├── test_leitura.py
    ├── test_processamento.py
```

## Contribuição

Contribuições são bem-vindas! Por favor, siga os passos abaixo:

1. Faça um fork do projeto.
2. Crie uma nova branch:
   ```bash
   git checkout -b minha-nova-funcionalidade
   ```
3. Faça as alterações desejadas e adicione testes.
4. Commit suas mudanças:
   ```bash
   git commit -m 'Adiciona nova funcionalidade'
   ```
5. Envie para a branch original:
   ```bash
   git push origin minha-nova-funcionalidade
   ```
6. Crie um pull request.

## Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
