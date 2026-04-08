# FUNCTIONAL_LIBRARY

Biblioteca utilitária simples com funcionalidades focadas em:

- salvamento de dados em arquivo (`salvar`)
- geração de texto ASCII art (`gerar_texto_gigante`)
- criação de bot Discord (`criar_bot`)
- comandos de moderação para Discord (`comandos_basicos`)
- download de vídeo (`baixar_video`)

## Instalação

```bash
pip install git+https://github.com/JoaoVitalPortugal/functional_library.git
```

## Uso

```python
import functional_library as fl

fl.salvar("teste")
print(fl.gerar_texto_gigante("oi", fonte="big"))

bot = fl.criar_bot("!")
fl.comandos_basicos(bot)

@bot.tree.command(name="ping", description="Responde Pong")
async def ping(interaction):
    await interaction.response.send_message("Pong")

bot.run("SEU_TOKEN")
```

## Dependências

- pyfiglet
- discord.py
- yt-dlp

## Autor

- Jovenzinho
