# llm-code-review-clojure

Respositório destinado à pesquisa intitulada "Otimização de Modelos LLM na revisão de código em Clojure" desenvolvida na Universidade Federal de Campina Grande (UFCG) entre 2023/2024 por meio do programa de Iniciação Científica PIBIC/CNPQ.

# Coleta de Dados
Para a realização da pesquisa foram coletados _pull requests_ de projetos _open source_ do _GitHub_, listados abaixo:

|Projeto                    |Respositório                                        |PRs  |
|---------------------------|----------------------------------------------------|-----|
|FiraCode                   |https://github.com/tonsky/FiraCode                  |183  |
|metabase                   |https://github.com/metabase/metabase                |20516|
|logseq                     |https://github.com/logseq/logseq                    |3071 |
|penpot                     |https://github.com/penpot/penpot                    |2441 |
|LightTable                 |https://github.com/LightTable/LightTable            |370  |
|clojurescript              |https://github.com/clojure/clojurescript            |177  |
|leiningen                  |https://github.com/technomancy/leiningen            |903  |
|om                         |https://github.com/omcljs/om                        |231  |
|jepsen                     |https://github.com/jepsen-io/jepsen                 |344  |
|athens                     |https://github.com/athensresearch/athens            |1386 |
|overtone                   |https://github.com/overtone/overtone                |192  |
|re-frame                   |https://github.com/day8/re-frame                    |458  |
|datascript                 |https://github.com/tonsky/datascript                |153  |
|reagent                    |https://github.com/reagent-project/reagent          |211  |
|riemann                    |https://github.com/riemann/riemann                  |631  |
|compojure                  |https://github.com/weavejester/compojure            |61   |
|icepick                    |https://github.com/frankiesardo/icepick             |27   |
|status-mobile              |https://github.com/status-im/status-mobile          |8936 |
|clojure-koans              |https://github.com/functional-koans/clojure-koans   |123  |
|ring                       |https://github.com/ring-clojure/ring                |237  |
|babashka                   |https://github.com/babashka/babashka                |706  |
|mori                       |https://github.com/swannodette/mori                 |85   |
|modern-cljs                |https://github.com/magomimmo/modern-cljs            |331  |
|quil                       |https://github.com/quil/quil                        |143  |
|lein-figwheel              |https://github.com/bhauman/lein-figwheel            |171  |
|swarmpit                   |https://github.com/swarmpit/swarmpit                |119  |
|instaparse                 |https://github.com/Engelberg/instaparse             |71   |
|pedestal                   |https://github.com/pedestal/pedestal                |368  |
|awesome-clojure            |https://github.com/razum2um/awesome-clojure         |172  |
|hiccup                     |https://github.com/weavejester/hiccup               |91   |
|clojure-cookbook           |https://github.com/clojure-cookbook/clojure-cookbook|397  |
|aleph                      |https://github.com/clj-commons/aleph                |341  |
|specter                    |https://github.com/redplanetlabs/specter            |59   |
|xtdb                       |https://github.com/xtdb/xtdb                        |1019 |
|schema                     |https://github.com/plumatic/schema                  |222  |
|code-math                  |https://github.com/adamtornhill/code-maat           |29   |
|incanter                   |https://github.com/incanter/incanter                |200  |
|shadow-cljs                |https://github.com/thheller/shadow-cljs             |126  |
|component                  |https://github.com/stuartsierra/component           |29   |
|onyx                       |https://github.com/onyx-platform/onyx               |307  |
|maelstrom                  |https://github.com/jepsen-io/maelstrom              |50   |
|core.async                 |https://github.com/clojure/core.async               |32   |
|lumo                       |https://github.com/anmonteiro/lumo                  |211  |
|transit-format             |https://github.com/cognitect/transit-format         |11   |
|lacinia                    |https://github.com/walmartlabs/lacinia              |263  |
|boot                       |https://github.com/boot-clj/boot                    |232  |
|clj-http                   |https://github.com/dakrone/clj-http                 |317  |
|kibit                      |https://github.com/clj-commons/kibit                |123  |
|sente                      |https://github.com/taoensso/sente                   |119  |
|midje                      |https://github.com/marick/Midje                     |129  |
|arcadia                    |https://github.com/arcadia-unity/Arcadia            |60   |
|honeysql                   |https://github.com/seancorfield/honeysql            |165  |
|clj-kondo                  |https://github.com/clj-kondo/clj-kondo              |886  |
|clerk                      |https://github.com/nextjournal/clerk                |358  |
|enlive                     |https://github.com/cgrand/enlive                    |64   |
|datahike                   |https://github.com/replikativ/datahike              |309  |
|devcards                   |https://github.com/bhauman/devcards                 |66   |
|fulcro                     |https://github.com/fulcrologic/fulcro               |257  |
|drake                      |https://github.com/Factual/drake                    |48   |
|plumbing                   |https://github.com/plumatic/plumbing                |81   |
|closh                      |https://github.com/dundalek/closh                   |47   |
|Korma                      |https://github.com/korma/Korma                      |165  |
|electric                   |https://github.com/hyperfiddle/electric             |22   |
|chesire                    |https://github.com/dakrone/cheshire                 |91   |
|konstellate                |https://github.com/jeremykross/konstellate          |6    |
|yesql                      |https://github.com/krisajenkins/yesql               |62   |
|seesaw                     |https://github.com/clj-commons/seesaw               |102  |
|timbre                     |https://github.com/taoensso/timbre                  |119  |
|core.logic                 |https://github.com/clojure/core.logic               |23   |
|Nightcode                  |https://github.com/oakes/Nightcode                  |47   |
|cascalog                   |https://github.com/nathanmarz/cascalog              |155  |
|auto-parcel                |https://github.com/frankiesardo/auto-parcel         |14   |
|reitit                     |https://github.com/metosin/reitit                   |345  |
|malli                      |https://github.com/metosin/malli                    |554  |
|garden                     |https://github.com/noprompt/garden                  |55   |
|duckling_old               |https://github.com/facebookarchive/duckling_old     |148  |
|chestnut                   |https://github.com/plexus/chestnut                  |117  |
|core.typed                 |https://github.com/clojure/core.typed               |32   |
|cortex                     |https://github.com/originrose/cortex                |195  |
|ClojureDart                |https://github.com/Tensegritics/ClojureDart         |106  |
|liberator                  |https://github.com/clojure-liberator/liberator      |158  |
|ultra                      |https://github.com/venantius/ultra                  |31   |
|dactyl-manuform            |https://github.com/abstracthat/dactyl-manuform      |1    |
|mount                      |https://github.com/tolitius/mount                   |42   |
|hitchhiker-tree            |https://github.com/datacrypt-project/hitchhiker-tree|20   |
|friend                     |https://github.com/cemerick/friend                  |61   |
|clara-rules                |https://github.com/cerner/clara-rules               |202  |
|core.match                 |https://github.com/clojure/core.match               |9    |
|integrant                  |https://github.com/weavejester/integrant            |38   |
|criterium                  |https://github.com/hugoduncan/criterium             |23   |
|frak                       |https://github.com/noprompt/frak                    |9    |
|sci                        |https://github.com/babashka/sci                     |393  |
|carmine                    |https://github.com/taoensso/carmine                 |74   |
|duct                       |https://github.com/duct-framework/duct              |36   |
|test.check                 |https://github.com/clojure/test.check               |16   |
|compojure-api              |https://github.com/metosin/compojure-api            |161  |
|cljs-devtools              |https://github.com/binaryage/cljs-devtools          |14   |
|lein-cljsbuild             |https://github.com/emezeske/lein-cljsbuild          |101  |
|eastwood                   |https://github.com/jonase/eastwood                  |119  |
|nubank: matcher-combinators|https://github.com/nubank/matcher-combinators/      |151  |
|nubank: workspaces         |https://github.com/nubank/workspaces                |44   |
|nubank: state-flow         |https://github.com/nubank/state-flow                |144  |
|                           |                                                    |     |
|Total de PRs               |                                                    |53331|

