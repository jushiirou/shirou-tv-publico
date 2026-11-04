# Materiais públicos do ShirouTV

Estes arquivos vão para um repositório público separado (por exemplo `jushiirou/shirou-tv-publico`, com GitHub Pages), para continuarem no ar mesmo se o repositório de versões ficar privado.

| Arquivo | Para quê |
|---|---|
| `teste.m3u` | Lista de teste, só com vídeos de licença livre. Cada item tem a licença anotada em comentário. |
| `privacidade.html` | Política de privacidade (link exigido pela Play Console). |
| `testadores.html` | Instruções para testadores, em português e inglês. |

## Marcadores a substituir antes de publicar

Procure e troque em `privacidade.html` e `testadores.html` (busca e substituição do editor):

- `EMAIL_SUPORTE` pelo e-mail de suporte (aparece em `mailto:EMAIL_SUPORTE` e no texto do link).
- `URL_LISTA` pelo endereço público do `teste.m3u`, por exemplo `https://jushiirou.github.io/shirou-tv-publico/teste.m3u`.

Depois confira que não sobrou nenhum marcador: `grep -rn "EMAIL_SUPORTE\|URL_LISTA" .`

## Limites da lista de teste

- O importador de M3U do app põe **todos** os itens em **Ao vivo**; o `group-title` só organiza as categorias. **Filmes e Séries só são preenchidos por fontes Xtream**, não por M3U. Por isso a lista de teste não consegue exercitar Filmes nem Séries (e não fingimos que sim).
- Para o revisor do Google e para os testadores, Ao vivo é a área que a lista cobre. Para mostrar Filmes e Séries nas capturas de tela seria preciso uma fonte Xtream própria com conteúdo livre.
- Os links apontam para servidores de terceiros (Internet Archive, download.blender.org, Mux, Unified Streaming). Se algum sair do ar, troque o link e revise a licença anotada. Verificados em 01/11/2026.

## Créditos / Credits

Todos os filmes são usados sem alterações. © Blender Foundation.

| Filme | Site | Licença |
|---|---|---|
| Big Buck Bunny | peach.blender.org | CC BY 3.0 - https://creativecommons.org/licenses/by/3.0/ |
| Sintel (trailer) | durian.blender.org | CC BY 3.0 - https://creativecommons.org/licenses/by/3.0/ |
| Tears of Steel | mango.blender.org | CC BY 3.0 - https://creativecommons.org/licenses/by/3.0/ |
| Elephants Dream | orange.blender.org | CC BY 2.5 - https://creativecommons.org/licenses/by/2.5/ |

As duas transmissões HLS de teste (Mux e Unified Streaming) exibem Big Buck Bunny e Tears of Steel, hospedadas por esses serviços como demonstração pública.
