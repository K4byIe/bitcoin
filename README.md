Bitcoin Noyau d'intégration/arbre d'étapes
=====================================

https://bitcoincore.org

Pour une version binaire immédiatement utilisable du logiciel Bitcoin Core, voir
https://bitcoincore.org/en/download/.

De plus amples informations sur Bitcoin Core sont disponibles dans le [dossier doc](/doc).

Qu'est-ce que Bitcoin ?
----------------

Le bitcoin est une monnaie numérique expérimentale qui permet des paiements instantanés
n'importe qui, n'importe où dans le monde. Bitcoin utilise la technologie peer-to-peer pour
sans autorité centrale : la gestion des transactions et l'émission de monnaie sont effectuées
collectivement par le réseau. Bitcoin Core est le nom de l'open source
un logiciel qui permet l'utilisation de cette monnaie.

Pour plus d'informations, consultez le livre blanc original de Bitcoin.

Licence
-------

Bitcoin Core est publié selon les termes de la licence du MIT. Voir [COPIE](COPYING) pour plus d'informations.
ou voir https://opensource.org/licenses/MIT.

Processus de développement
-------------------

La branche "maître" est régulièrement construite (voir "doc/build-*.md" pour les instructions) et testée, mais il n'est pas garanti qu'elle soit
complètement stable. [Tags](https://github.com/bitcoin/bitcoin/tags) sont créés
régulièrement des branches de publication pour indiquer les nouvelles versions officielles et stables de Bitcoin Core.

Le dépôt https://github.com/bitcoin-core/gui est utilisé exclusivement pour le
développement de l'interface graphique. Sa branche maîtresse est identique dans tous les monotones
des dépôts. Les branches et les balises de libération n'existent pas, alors veuillez ne pas bifurquer
ce dépôt, sauf si c'est pour des raisons de développement.

Le déroulement des contributions est décrit dans [CONTRIBUTING.md](CONTRIBUTING.md)
et des conseils utiles pour les développeurs peuvent être trouvés dans [doc/developer-notes.md](doc/developer-notes.md).

Test
-------

Les essais et la révision des codes sont le goulot d'étranglement du développement ; nous obtenons plus de poids
que nous pouvons examiner et tester à court terme. Veuillez être patient et nous aider en testant
les demandes d'extraction d'autres personnes, et n'oubliez pas qu'il s'agit d'un projet essentiel pour la sécurité, où toute erreur pourrait coûter cher
beaucoup d'argent.

### Tests automatisés

Les développeurs sont fortement encouragés à écrire [tests unitaires] (src/test/README.md) pour le nouveau code, et à
soumettre de nouveaux tests unitaires pour l'ancien code. Les tests unitaires peuvent être compilés et exécutés
(en supposant qu'ils n'aient pas été désactivés dans le configurateur) avec : "make check". Plus de détails sur l'exécution de
et l'extension des tests unitaires se trouvent dans [/src/test/README.md](/src/test/README.md).

Il existe également des [tests de régression et d'intégration](/test), écrits
en Python.
Ces tests peuvent être exécutés (si les [dépendances de test](/test) sont installées) avec : `test/functional/test_runner.py`

Les systèmes CI (Continuous Integration) s'assurent que chaque demande d'extraction est construite pour Windows, Linux et macOS,
et que les tests d'unité/sanité sont effectués automatiquement.

### Tests manuels d'assurance qualité (AQ)

Les modifications doivent être testées par une personne autre que le développeur qui a écrit le
code. Ceci est particulièrement important pour les changements importants ou à haut risque. Il est utile
d'ajouter un plan d'essai à la description de la demande de retrait si l'essai des modifications est
pas simple.

Traductions
------------

Les modifications des traductions ainsi que les nouvelles traductions peuvent être soumises à
[page Transifex de Bitcoin Core] (https://www.transifex.com/bitcoin/bitcoin/).

Les traductions sont périodiquement extraites de Transifex et fusionnées dans le dépôt git. Voir la page
[processus de traduction](doc/translation_process.md) pour plus de détails sur le fonctionnement.

**Important** : Nous n'acceptons pas les changements de traduction comme des demandes de GitHub pull car la prochaine
de Transifex les écraserait automatiquement à nouveau.


Traduit avec par 4po
