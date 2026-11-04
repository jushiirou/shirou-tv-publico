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

- O app separa os itens da lista M3U: os **filmes** (links `/movie/` ou arquivos de vídeo como `.mp4`, `.mkv`, `.mov`) vão para **Filmes**; o resto fica em **Ao vivo**. Os **episódios** (links `/series/` ou nomes como "S01E02") viram **Séries**. Com esta lista: 2 transmissões em Ao vivo, 4 filmes em Filmes e 1 série (Caminandes, 3 episódios) em Séries.
- Para o revisor do Google e para os testadores, a lista cobre Ao vivo, Filmes e Séries.
- Os links apontam para servidores de terceiros (Internet Archive, download.blender.org, Mux, Unified Streaming). Se algum sair do ar, troque o link e revise a licença anotada. Verificados em 01/11/2026.

## Créditos / Credits

Todos os filmes são usados sem alterações. © Blender Foundation.

| Filme | Site | Licença |
|---|---|---|
| Big Buck Bunny | peach.blender.org | CC BY 3.0 - https://creativecommons.org/licenses/by/3.0/ |
| Sintel (trailer) | durian.blender.org | CC BY 3.0 - https://creativecommons.org/licenses/by/3.0/ |
| Tears of Steel | mango.blender.org | CC BY 3.0 - https://creativecommons.org/licenses/by/3.0/ |
| Elephants Dream | orange.blender.org | CC BY 2.5 - https://creativecommons.org/licenses/by/2.5/ |
| Caminandes (Llama Drama, Gran Dillama, Llamigos) | caminandes.com (Pablo Vazquez / Blender Foundation) | CC BY 3.0 - https://creativecommons.org/licenses/by/3.0/ |

As duas transmissões HLS de teste (Mux e Unified Streaming) exibem Big Buck Bunny e Tears of Steel, hospedadas por esses serviços como demonstração pública.
