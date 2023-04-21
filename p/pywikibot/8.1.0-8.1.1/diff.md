# Comparing `tmp/pywikibot-8.1.0.tar.gz` & `tmp/pywikibot-8.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywikibot-8.1.0.tar", last modified: Sun Apr 16 15:00:32 2023, max compression
+gzip compressed data, was "pywikibot-8.1.1.tar", last modified: Fri Apr 21 08:21:51 2023, max compression
```

## Comparing `pywikibot-8.1.0.tar` & `pywikibot-8.1.1.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:32.257337 pywikibot-8.1.0/
--rw-rw-rw-   0        0        0     4115 2023-04-10 16:20:49.000000 pywikibot-8.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     1086 2023-04-10 16:20:49.000000 pywikibot-8.1.0/LICENSE
--rw-rw-rw-   0        0        0       40 2023-04-10 16:20:49.000000 pywikibot-8.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    15494 2023-04-16 15:00:32.257337 pywikibot-8.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5495 2023-04-10 16:20:49.000000 pywikibot-8.1.0/README.rst
--rw-rw-rw-   0        0        0     6351 2023-04-16 15:00:25.000000 pywikibot-8.1.0/make_dist.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:30.905407 pywikibot-8.1.0/pywikibot/
--rw-rw-rw-   0        0        0    55820 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/__init__.py
--rw-rw-rw-   0        0        0      794 2023-04-16 13:54:05.000000 pywikibot-8.1.0/pywikibot/__metadata__.py
--rw-rw-rw-   0        0        0     1886 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/_wbtypes.py
--rw-rw-rw-   0        0        0     4476 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/backports.py
--rw-rw-rw-   0        0        0    96117 2023-04-14 14:19:20.000000 pywikibot-8.1.0/pywikibot/bot.py
--rw-rw-rw-   0        0        0    21207 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/bot_choice.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:30.956314 pywikibot-8.1.0/pywikibot/comms/
--rw-rw-rw-   0        0        0      121 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/comms/__init__.py
--rw-rw-rw-   0        0        0    15749 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/comms/eventstreams.py
--rw-rw-rw-   0        0        0    19597 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/comms/http.py
--rw-rw-rw-   0        0        0    46527 2023-04-14 14:19:20.000000 pywikibot-8.1.0/pywikibot/config.py
--rw-rw-rw-   0        0        0    46135 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/cosmetic_changes.py
--rw-rw-rw-   0        0        0     2090 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/daemonize.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.006224 pywikibot-8.1.0/pywikibot/data/
--rw-rw-rw-   0        0        0      160 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.055135 pywikibot-8.1.0/pywikibot/data/api/
--rw-rw-rw-   0        0        0     3174 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/api/__init__.py
--rw-rw-rw-   0        0        0    41816 2023-04-14 14:19:36.000000 pywikibot-8.1.0/pywikibot/data/api/_generators.py
--rw-rw-rw-   0        0        0     7398 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/api/_optionset.py
--rw-rw-rw-   0        0        0    23233 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/api/_paraminfo.py
--rw-rw-rw-   0        0        0    52510 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/data/api/_requests.py
--rw-rw-rw-   0        0        0    14143 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/memento.py
--rw-rw-rw-   0        0        0     2919 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/mysql.py
--rw-rw-rw-   0        0        0     8969 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/sparql.py
--rw-rw-rw-   0        0        0     3970 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/wikistats.py
--rw-rw-rw-   0        0        0    96940 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/date.py
--rw-rw-rw-   0        0        0    24879 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/diff.py
--rw-rw-rw-   0        0        0     2054 2023-04-15 09:05:00.000000 pywikibot-8.1.0/pywikibot/echo.py
--rw-rw-rw-   0        0        0     7830 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/editor.py
--rw-rw-rw-   0        0        0    21221 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.287712 pywikibot-8.1.0/pywikibot/families/
--rw-rw-rw-   0        0        0      118 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/__init__.py
--rw-rw-rw-   0        0        0     4303 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/commons_family.py
--rw-rw-rw-   0        0        0      443 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/foundation_family.py
--rw-rw-rw-   0        0        0      463 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/i18n_family.py
--rw-rw-rw-   0        0        0      355 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/incubator_family.py
--rw-rw-rw-   0        0        0      662 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/lingualibre_family.py
--rw-rw-rw-   0        0        0      401 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/mediawiki_family.py
--rw-rw-rw-   0        0        0      593 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/meta_family.py
--rw-rw-rw-   0        0        0     1330 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/osm_family.py
--rw-rw-rw-   0        0        0      369 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/outreach_family.py
--rw-rw-rw-   0        0        0      361 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/species_family.py
--rw-rw-rw-   0        0        0      638 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/vikidia_family.py
--rw-rw-rw-   0        0        0     2418 2023-04-16 13:54:05.000000 pywikibot-8.1.0/pywikibot/families/wikibooks_family.py
--rw-rw-rw-   0        0        0     3782 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikidata_family.py
--rw-rw-rw-   0        0        0     1742 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikihow_family.py
--rw-rw-rw-   0        0        0     1009 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikimania_family.py
--rw-rw-rw-   0        0        0      777 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikimediachapter_family.py
--rw-rw-rw-   0        0        0     1825 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikinews_family.py
--rw-rw-rw-   0        0        0    10730 2023-04-16 13:54:05.000000 pywikibot-8.1.0/pywikibot/families/wikipedia_family.py
--rw-rw-rw-   0        0        0     2886 2023-04-16 13:54:05.000000 pywikibot-8.1.0/pywikibot/families/wikiquote_family.py
--rw-rw-rw-   0        0        0     5335 2023-04-16 13:54:05.000000 pywikibot-8.1.0/pywikibot/families/wikisource_family.py
--rw-rw-rw-   0        0        0      495 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikispore_family.py
--rw-rw-rw-   0        0        0      425 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikitech_family.py
--rw-rw-rw-   0        0        0     1150 2023-04-14 14:19:20.000000 pywikibot-8.1.0/pywikibot/families/wikiversity_family.py
--rw-rw-rw-   0        0        0     1027 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikivoyage_family.py
--rw-rw-rw-   0        0        0     3827 2023-04-16 13:54:05.000000 pywikibot-8.1.0/pywikibot/families/wiktionary_family.py
--rw-rw-rw-   0        0        0     2404 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wowwiki_family.py
--rw-rw-rw-   0        0        0    37565 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/family.py
--rw-rw-rw-   0        0        0    33191 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/fixes.py
--rw-rw-rw-   0        0        0    20119 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/flow.py
--rw-rw-rw-   0        0        0    30038 2023-04-14 14:19:20.000000 pywikibot-8.1.0/pywikibot/i18n.py
--rw-rw-rw-   0        0        0     8343 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/interwiki_graph.py
--rw-rw-rw-   0        0        0    13245 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/logentries.py
--rw-rw-rw-   0        0        0    12508 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/logging.py
--rw-rw-rw-   0        0        0    22781 2023-04-14 14:19:20.000000 pywikibot-8.1.0/pywikibot/login.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.407494 pywikibot-8.1.0/pywikibot/page/
--rw-rw-rw-   0        0        0     2350 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/__init__.py
--rw-rw-rw-   0        0        0    86912 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/page/_basepage.py
--rw-rw-rw-   0        0        0    14617 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_category.py
--rw-rw-rw-   0        0        0    19000 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_collections.py
--rw-rw-rw-   0        0        0     2183 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_decorators.py
--rw-rw-rw-   0        0        0    14648 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_filepage.py
--rw-rw-rw-   0        0        0    29601 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_links.py
--rw-rw-rw-   0        0        0     8515 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_page.py
--rw-rw-rw-   0        0        0     2997 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_revision.py
--rw-rw-rw-   0        0        0     4049 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_toolforge.py
--rw-rw-rw-   0        0        0    16348 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_user.py
--rw-rw-rw-   0        0        0    86381 2023-04-15 09:05:00.000000 pywikibot-8.1.0/pywikibot/page/_wikibase.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.453410 pywikibot-8.1.0/pywikibot/pagegenerators/
--rw-rw-rw-   0        0        0    29164 2023-04-14 16:24:14.000000 pywikibot-8.1.0/pywikibot/pagegenerators/__init__.py
--rw-rw-rw-   0        0        0    40342 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/pagegenerators/_factory.py
--rw-rw-rw-   0        0        0    19272 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/pagegenerators/_filters.py
--rw-rw-rw-   0        0        0    44438 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/pagegenerators/_generators.py
--rw-rw-rw-   0        0        0     3938 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/plural.py
--rw-rw-rw-   0        0        0    48967 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/proofreadpage.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.516298 pywikibot-8.1.0/pywikibot/scripts/
--rw-rw-rw-   0        0        0      882 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/__init__.py
--rw-rw-rw-   0        0        0    11972 2023-04-16 09:28:42.000000 pywikibot-8.1.0/pywikibot/scripts/generate_family_file.py
--rw-rw-rw-   0        0        0    19989 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/generate_user_files.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.523283 pywikibot-8.1.0/pywikibot/scripts/i18n/
--rw-rw-rw-   0        0        0      309 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.938529 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/
--rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ab.json
--rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/af.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/an.json
--rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ar.json
--rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/arc.json
--rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ast.json
--rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/av.json
--rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/awa.json
--rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/az.json
--rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/azb.json
--rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ba.json
--rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bar.json
--rw-rw-rw-   0        0        0      989 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bcc.json
--rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/be-tarask.json
--rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/be.json
--rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bg.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bjn.json
--rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bn.json
--rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bo.json
--rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/br.json
--rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bs.json
--rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ca.json
--rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ce.json
--rw-rw-rw-   0        0        0      768 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ckb.json
--rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/cs.json
--rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/csb.json
--rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/cy.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/da.json
--rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/de.json
--rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/diq.json
--rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/el.json
--rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/en.json
--rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/eo.json
--rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/es.json
--rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/et.json
--rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/eu.json
--rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fa.json
--rw-rw-rw-   0        0        0      660 2022-04-15 15:42:25.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fi.json
--rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fo.json
--rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fr.json
--rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/frp.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/frr.json
--rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fy.json
--rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ga.json
--rw-rw-rw-   0        0        0     1082 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/gl.json
--rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/gsw.json
--rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hak.json
--rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/haw.json
--rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/he.json
--rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hi.json
--rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hr.json
--rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hsb.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hu.json
--rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hy.json
--rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ia.json
--rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/id.json
--rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ie.json
--rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ig.json
--rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ilo.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/io.json
--rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/is.json
--rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/it.json
--rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ja.json
--rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/jv.json
--rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/kab.json
--rw-rw-rw-   0        0        0     1068 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/kk.json
--rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/km.json
--rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/kn.json
--rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ko.json
--rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/krc.json
--rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ksh.json
--rw-rw-rw-   0        0        0      318 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ku.json
--rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ky.json
--rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/la.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/lb.json
--rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/li.json
--rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/lki.json
--rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/lt.json
--rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/lv.json
--rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/map-bms.json
--rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/mg.json
--rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/min.json
--rw-rw-rw-   0        0        0     1353 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/mk.json
--rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ml.json
--rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/mni.json
--rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/mr.json
--rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ms.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/mt.json
--rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/my.json
--rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nan.json
--rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nb.json
--rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nds-nl.json
--rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nds.json
--rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ne.json
--rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/new.json
--rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nl.json
--rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nn.json
--rw-rw-rw-   0        0        0     1344 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nqo.json
--rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nyn.json
--rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/oc.json
--rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/olo.json
--rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/or.json
--rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pa.json
--rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pdc.json
--rw-rw-rw-   0        0        0      102 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pfl.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pl.json
--rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pms.json
--rw-rw-rw-   0        0        0     1070 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pt-br.json
--rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pt.json
--rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/qqq.json
--rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ro.json
--rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ru.json
--rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/scn.json
--rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sco.json
--rw-rw-rw-   0        0        0      311 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sd.json
--rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sh.json
--rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/si.json
--rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sk.json
--rw-rw-rw-   0        0        0      193 2023-04-06 12:04:37.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/skr-arab.json
--rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sl.json
--rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sms.json
--rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/so.json
--rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sq.json
--rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sr.json
--rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/su.json
--rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sv.json
--rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sw.json
--rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/szl.json
--rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ta.json
--rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/te.json
--rw-rw-rw-   0        0        0      101 2023-04-06 12:04:37.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tg.json
--rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/th.json
--rw-rw-rw-   0        0        0      155 2023-04-06 12:04:37.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tk.json
--rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tl.json
--rw-rw-rw-   0        0        0     1115 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tly.json
--rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tr.json
--rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tt.json
--rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/uk.json
--rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ur.json
--rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/uz.json
--rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/vec.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/vep.json
--rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/vi.json
--rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/vo.json
--rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/war.json
--rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/yi.json
--rw-rw-rw-   0        0        0      850 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/yue.json
--rw-rw-rw-   0        0        0     1084 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/zh.json
--rw-rw-rw-   0        0        0     6093 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/login.py
--rw-rw-rw-   0        0        0     3246 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/preload_sites.py
--rw-rw-rw-   0        0        0     1791 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/shell.py
--rw-rw-rw-   0        0        0     3313 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/version.py
--rw-rw-rw-   0        0        0    18491 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:32.061304 pywikibot-8.1.0/pywikibot/site/
--rw-rw-rw-   0        0        0      744 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/__init__.py
--rw-rw-rw-   0        0        0   112500 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/site/_apisite.py
--rw-rw-rw-   0        0        0    15864 2023-04-15 09:05:00.000000 pywikibot-8.1.0/pywikibot/site/_basesite.py
--rw-rw-rw-   0        0        0    38276 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_datasite.py
--rw-rw-rw-   0        0        0     4254 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_decorators.py
--rw-rw-rw-   0        0        0    27978 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_extensions.py
--rw-rw-rw-   0        0        0    93641 2023-04-14 16:24:14.000000 pywikibot-8.1.0/pywikibot/site/_generators.py
--rw-rw-rw-   0        0        0     3003 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_interwikimap.py
--rw-rw-rw-   0        0        0    14558 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_namespace.py
--rw-rw-rw-   0        0        0     1667 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_obsoletesites.py
--rw-rw-rw-   0        0        0    14354 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_siteinfo.py
--rw-rw-rw-   0        0        0     4868 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/site/_tokenwallet.py
--rw-rw-rw-   0        0        0    25321 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_upload.py
--rw-rw-rw-   0        0        0    11231 2023-04-16 10:49:33.000000 pywikibot-8.1.0/pywikibot/site_detect.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:32.085649 pywikibot-8.1.0/pywikibot/specialbots/
--rw-rw-rw-   0        0        0      371 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/specialbots/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/specialbots/_unlink.py
--rw-rw-rw-   0        0        0    20247 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/specialbots/_upload.py
--rw-rw-rw-   0        0        0    84825 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/textlib.py
--rw-rw-rw-   0        0        0    12074 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/throttle.py
--rw-rw-rw-   0        0        0    15061 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/time.py
--rw-rw-rw-   0        0        0     3267 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/titletranslate.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:32.175486 pywikibot-8.1.0/pywikibot/tools/
--rw-rw-rw-   0        0        0    27088 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/__init__.py
--rw-rw-rw-   0        0        0    25467 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/_deprecate.py
--rw-rw-rw-   0        0        0     1205 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/_logging.py
--rw-rw-rw-   0        0        0    22207 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/_unidata.py
--rw-rw-rw-   0        0        0     3116 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/chars.py
--rw-rw-rw-   0        0        0     8765 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/collections.py
--rw-rw-rw-   0        0        0    11075 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/djvu.py
--rw-rw-rw-   0        0        0     4021 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/formatter.py
--rw-rw-rw-   0        0        0     9745 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/itertools.py
--rw-rw-rw-   0        0        0     7334 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/threading.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:32.246357 pywikibot-8.1.0/pywikibot/userinterfaces/
--rw-rw-rw-   0        0        0      870 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/__init__.py
--rw-rw-rw-   0        0        0     1906 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/_interface_base.py
--rw-rw-rw-   0        0        0     2687 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/buffer_interface.py
--rw-rw-rw-   0        0        0    22100 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/userinterfaces/gui.py
--rw-rw-rw-   0        0        0      457 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/terminal_interface.py
--rw-rw-rw-   0        0        0    24536 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/terminal_interface_base.py
--rw-rw-rw-   0        0        0     2114 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/terminal_interface_unix.py
--rw-rw-rw-   0        0        0     2012 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/terminal_interface_win32.py
--rw-rw-rw-   0        0        0    90310 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/transliteration.py
--rw-rw-rw-   0        0        0    16698 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/version.py
--rw-rw-rw-   0        0        0     7366 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/xmlreader.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:30.933357 pywikibot-8.1.0/pywikibot.egg-info/
--rw-rw-rw-   0        0        0    15494 2023-04-16 15:00:30.000000 pywikibot-8.1.0/pywikibot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10447 2023-04-16 15:00:30.000000 pywikibot-8.1.0/pywikibot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 15:00:30.000000 pywikibot-8.1.0/pywikibot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-04-16 15:00:30.000000 pywikibot-8.1.0/pywikibot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1228 2023-04-16 15:00:30.000000 pywikibot-8.1.0/pywikibot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-16 15:00:30.000000 pywikibot-8.1.0/pywikibot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 15:00:32.257337 pywikibot-8.1.0/setup.cfg
--rw-rw-rw-   0        0        0    13116 2023-04-15 09:02:53.000000 pywikibot-8.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:00:32.255340 pywikibot-8.1.0/tests/
--rw-rw-rw-   0        0        0     2814 2023-04-14 09:45:27.000000 pywikibot-8.1.0/tests/tests_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.591101 pywikibot-8.1.1/
+-rw-rw-rw-   0        0        0     4115 2023-04-10 16:20:49.000000 pywikibot-8.1.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1086 2023-04-10 16:20:49.000000 pywikibot-8.1.1/LICENSE
+-rw-rw-rw-   0        0        0       40 2023-04-10 16:20:49.000000 pywikibot-8.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    14586 2023-04-21 08:21:51.589108 pywikibot-8.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5495 2023-04-10 16:20:49.000000 pywikibot-8.1.1/README.rst
+-rw-rw-rw-   0        0        0     6351 2023-04-16 15:04:28.000000 pywikibot-8.1.1/make_dist.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:50.974750 pywikibot-8.1.1/pywikibot/
+-rw-rw-rw-   0        0        0    55820 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/__init__.py
+-rw-rw-rw-   0        0        0      794 2023-04-21 07:37:30.000000 pywikibot-8.1.1/pywikibot/__metadata__.py
+-rw-rw-rw-   0        0        0     1886 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/_wbtypes.py
+-rw-rw-rw-   0        0        0     4476 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/backports.py
+-rw-rw-rw-   0        0        0    96117 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/bot.py
+-rw-rw-rw-   0        0        0    21207 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/bot_choice.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:50.998685 pywikibot-8.1.1/pywikibot/comms/
+-rw-rw-rw-   0        0        0      121 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/comms/__init__.py
+-rw-rw-rw-   0        0        0    15749 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/comms/eventstreams.py
+-rw-rw-rw-   0        0        0    19597 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/comms/http.py
+-rw-rw-rw-   0        0        0    46527 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/config.py
+-rw-rw-rw-   0        0        0    46135 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/cosmetic_changes.py
+-rw-rw-rw-   0        0        0     2090 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/daemonize.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.005666 pywikibot-8.1.1/pywikibot/data/
+-rw-rw-rw-   0        0        0      160 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.012647 pywikibot-8.1.1/pywikibot/data/api/
+-rw-rw-rw-   0        0        0     3174 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/api/__init__.py
+-rw-rw-rw-   0        0        0    41816 2023-04-14 14:19:36.000000 pywikibot-8.1.1/pywikibot/data/api/_generators.py
+-rw-rw-rw-   0        0        0     7398 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/api/_optionset.py
+-rw-rw-rw-   0        0        0    23233 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/api/_paraminfo.py
+-rw-rw-rw-   0        0        0    52512 2023-04-16 16:10:48.000000 pywikibot-8.1.1/pywikibot/data/api/_requests.py
+-rw-rw-rw-   0        0        0    14143 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/memento.py
+-rw-rw-rw-   0        0        0     2919 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/mysql.py
+-rw-rw-rw-   0        0        0     8969 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/sparql.py
+-rw-rw-rw-   0        0        0     3970 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/wikistats.py
+-rw-rw-rw-   0        0        0    96940 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/date.py
+-rw-rw-rw-   0        0        0    24879 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/diff.py
+-rw-rw-rw-   0        0        0     2042 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/echo.py
+-rw-rw-rw-   0        0        0     7830 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/editor.py
+-rw-rw-rw-   0        0        0    21221 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.047566 pywikibot-8.1.1/pywikibot/families/
+-rw-rw-rw-   0        0        0      118 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/__init__.py
+-rw-rw-rw-   0        0        0     4303 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/commons_family.py
+-rw-rw-rw-   0        0        0      443 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/foundation_family.py
+-rw-rw-rw-   0        0        0      463 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/i18n_family.py
+-rw-rw-rw-   0        0        0      355 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/incubator_family.py
+-rw-rw-rw-   0        0        0      662 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/lingualibre_family.py
+-rw-rw-rw-   0        0        0      401 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/mediawiki_family.py
+-rw-rw-rw-   0        0        0      593 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/meta_family.py
+-rw-rw-rw-   0        0        0     1330 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/osm_family.py
+-rw-rw-rw-   0        0        0      369 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/outreach_family.py
+-rw-rw-rw-   0        0        0      361 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/species_family.py
+-rw-rw-rw-   0        0        0      638 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/vikidia_family.py
+-rw-rw-rw-   0        0        0     2418 2023-04-16 15:09:16.000000 pywikibot-8.1.1/pywikibot/families/wikibooks_family.py
+-rw-rw-rw-   0        0        0     3782 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/wikidata_family.py
+-rw-rw-rw-   0        0        0     1742 2023-04-18 14:17:02.000000 pywikibot-8.1.1/pywikibot/families/wikihow_family.py
+-rw-rw-rw-   0        0        0     1009 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/wikimania_family.py
+-rw-rw-rw-   0        0        0      777 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/wikimediachapter_family.py
+-rw-rw-rw-   0        0        0     1825 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/wikinews_family.py
+-rw-rw-rw-   0        0        0    10737 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/families/wikipedia_family.py
+-rw-rw-rw-   0        0        0     2886 2023-04-21 05:58:04.000000 pywikibot-8.1.1/pywikibot/families/wikiquote_family.py
+-rw-rw-rw-   0        0        0     5335 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/families/wikisource_family.py
+-rw-rw-rw-   0        0        0      495 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/wikispore_family.py
+-rw-rw-rw-   0        0        0      425 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/wikitech_family.py
+-rw-rw-rw-   0        0        0     1150 2023-04-14 14:19:20.000000 pywikibot-8.1.1/pywikibot/families/wikiversity_family.py
+-rw-rw-rw-   0        0        0     1027 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/wikivoyage_family.py
+-rw-rw-rw-   0        0        0     3843 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/families/wiktionary_family.py
+-rw-rw-rw-   0        0        0     2414 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/families/wowwiki_family.py
+-rw-rw-rw-   0        0        0    37565 2023-04-18 14:17:02.000000 pywikibot-8.1.1/pywikibot/family.py
+-rw-rw-rw-   0        0        0    33191 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/fixes.py
+-rw-rw-rw-   0        0        0    20119 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/flow.py
+-rw-rw-rw-   0        0        0    30038 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/i18n.py
+-rw-rw-rw-   0        0        0     8343 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/interwiki_graph.py
+-rw-rw-rw-   0        0        0    13245 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/logentries.py
+-rw-rw-rw-   0        0        0    12508 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/logging.py
+-rw-rw-rw-   0        0        0    22781 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/login.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.066504 pywikibot-8.1.1/pywikibot/page/
+-rw-rw-rw-   0        0        0     2350 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/__init__.py
+-rw-rw-rw-   0        0        0    86912 2023-04-17 14:18:54.000000 pywikibot-8.1.1/pywikibot/page/_basepage.py
+-rw-rw-rw-   0        0        0    14617 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_category.py
+-rw-rw-rw-   0        0        0    19000 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_collections.py
+-rw-rw-rw-   0        0        0     2183 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_decorators.py
+-rw-rw-rw-   0        0        0    14648 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_filepage.py
+-rw-rw-rw-   0        0        0    29601 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_links.py
+-rw-rw-rw-   0        0        0     8515 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_page.py
+-rw-rw-rw-   0        0        0     2997 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_revision.py
+-rw-rw-rw-   0        0        0     4049 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_toolforge.py
+-rw-rw-rw-   0        0        0    16348 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_user.py
+-rw-rw-rw-   0        0        0    86375 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/page/_wikibase.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.071504 pywikibot-8.1.1/pywikibot/pagegenerators/
+-rw-rw-rw-   0        0        0    29164 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/pagegenerators/__init__.py
+-rw-rw-rw-   0        0        0    40342 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/pagegenerators/_factory.py
+-rw-rw-rw-   0        0        0    19272 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/pagegenerators/_filters.py
+-rw-rw-rw-   0        0        0    44438 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/pagegenerators/_generators.py
+-rw-rw-rw-   0        0        0     3938 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/plural.py
+-rw-rw-rw-   0        0        0    48967 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/proofreadpage.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.084456 pywikibot-8.1.1/pywikibot/scripts/
+-rw-rw-rw-   0        0        0      882 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/scripts/__init__.py
+-rw-rw-rw-   0        0        0    12032 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/scripts/generate_family_file.py
+-rw-rw-rw-   0        0        0    20029 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/scripts/generate_user_files.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.086450 pywikibot-8.1.1/pywikibot/scripts/i18n/
+-rw-rw-rw-   0        0        0      309 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.538241 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/
+-rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ab.json
+-rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/af.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/an.json
+-rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ar.json
+-rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/arc.json
+-rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ast.json
+-rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/av.json
+-rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/awa.json
+-rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/az.json
+-rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/azb.json
+-rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ba.json
+-rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bar.json
+-rw-rw-rw-   0        0        0      989 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bcc.json
+-rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/be-tarask.json
+-rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/be.json
+-rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bg.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bjn.json
+-rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bn.json
+-rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bo.json
+-rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/br.json
+-rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bs.json
+-rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ca.json
+-rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ce.json
+-rw-rw-rw-   0        0        0      768 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ckb.json
+-rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/cs.json
+-rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/csb.json
+-rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/cy.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/da.json
+-rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/de.json
+-rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/diq.json
+-rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/el.json
+-rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/en.json
+-rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/eo.json
+-rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/es.json
+-rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/et.json
+-rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/eu.json
+-rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fa.json
+-rw-rw-rw-   0        0        0      660 2022-04-15 15:42:25.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fi.json
+-rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fo.json
+-rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fr.json
+-rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/frp.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/frr.json
+-rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fy.json
+-rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ga.json
+-rw-rw-rw-   0        0        0     1082 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/gl.json
+-rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/gsw.json
+-rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hak.json
+-rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/haw.json
+-rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/he.json
+-rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hi.json
+-rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hr.json
+-rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hsb.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hu.json
+-rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hy.json
+-rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ia.json
+-rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/id.json
+-rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ie.json
+-rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ig.json
+-rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ilo.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/io.json
+-rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/is.json
+-rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/it.json
+-rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ja.json
+-rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/jv.json
+-rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/kab.json
+-rw-rw-rw-   0        0        0     1068 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/kk.json
+-rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/km.json
+-rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/kn.json
+-rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ko.json
+-rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/krc.json
+-rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ksh.json
+-rw-rw-rw-   0        0        0      318 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ku.json
+-rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ky.json
+-rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/la.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/lb.json
+-rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/li.json
+-rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/lki.json
+-rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/lt.json
+-rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/lv.json
+-rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/map-bms.json
+-rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/mg.json
+-rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/min.json
+-rw-rw-rw-   0        0        0     1353 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/mk.json
+-rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ml.json
+-rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/mni.json
+-rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/mr.json
+-rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ms.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/mt.json
+-rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/my.json
+-rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nan.json
+-rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nb.json
+-rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nds-nl.json
+-rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nds.json
+-rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ne.json
+-rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/new.json
+-rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nl.json
+-rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nn.json
+-rw-rw-rw-   0        0        0     1344 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nqo.json
+-rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nyn.json
+-rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/oc.json
+-rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/olo.json
+-rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/or.json
+-rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pa.json
+-rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pdc.json
+-rw-rw-rw-   0        0        0      102 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pfl.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pl.json
+-rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pms.json
+-rw-rw-rw-   0        0        0     1070 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pt-br.json
+-rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pt.json
+-rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/qqq.json
+-rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ro.json
+-rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ru.json
+-rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/scn.json
+-rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sco.json
+-rw-rw-rw-   0        0        0      311 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sd.json
+-rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sh.json
+-rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/si.json
+-rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sk.json
+-rw-rw-rw-   0        0        0      193 2023-04-06 12:04:37.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/skr-arab.json
+-rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sl.json
+-rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sms.json
+-rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/so.json
+-rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sq.json
+-rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sr.json
+-rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/su.json
+-rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sv.json
+-rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sw.json
+-rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/szl.json
+-rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ta.json
+-rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/te.json
+-rw-rw-rw-   0        0        0      101 2023-04-06 12:04:37.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tg.json
+-rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/th.json
+-rw-rw-rw-   0        0        0      155 2023-04-06 12:04:37.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tk.json
+-rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tl.json
+-rw-rw-rw-   0        0        0     1115 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tly.json
+-rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tr.json
+-rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tt.json
+-rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/uk.json
+-rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ur.json
+-rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/uz.json
+-rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/vec.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/vep.json
+-rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/vi.json
+-rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/vo.json
+-rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/war.json
+-rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/yi.json
+-rw-rw-rw-   0        0        0      850 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/yue.json
+-rw-rw-rw-   0        0        0     1084 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/zh.json
+-rw-rw-rw-   0        0        0     6093 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/scripts/login.py
+-rw-rw-rw-   0        0        0     3246 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/scripts/preload_sites.py
+-rw-rw-rw-   0        0        0     1791 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/scripts/shell.py
+-rw-rw-rw-   0        0        0     3313 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/scripts/version.py
+-rw-rw-rw-   0        0        0    18491 2023-04-20 07:19:22.000000 pywikibot-8.1.1/pywikibot/scripts/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.558189 pywikibot-8.1.1/pywikibot/site/
+-rw-rw-rw-   0        0        0      744 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/__init__.py
+-rw-rw-rw-   0        0        0   112506 2023-04-16 16:10:48.000000 pywikibot-8.1.1/pywikibot/site/_apisite.py
+-rw-rw-rw-   0        0        0    15858 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/site/_basesite.py
+-rw-rw-rw-   0        0        0    38276 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/_datasite.py
+-rw-rw-rw-   0        0        0     4254 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/_decorators.py
+-rw-rw-rw-   0        0        0    27978 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/_extensions.py
+-rw-rw-rw-   0        0        0    93641 2023-04-17 14:52:33.000000 pywikibot-8.1.1/pywikibot/site/_generators.py
+-rw-rw-rw-   0        0        0     3003 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/_interwikimap.py
+-rw-rw-rw-   0        0        0    14558 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/_namespace.py
+-rw-rw-rw-   0        0        0     1667 2023-04-18 14:53:43.000000 pywikibot-8.1.1/pywikibot/site/_obsoletesites.py
+-rw-rw-rw-   0        0        0    14354 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/_siteinfo.py
+-rw-rw-rw-   0        0        0     4868 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/site/_tokenwallet.py
+-rw-rw-rw-   0        0        0    25321 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/_upload.py
+-rw-rw-rw-   0        0        0    11156 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/site_detect.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.565171 pywikibot-8.1.1/pywikibot/specialbots/
+-rw-rw-rw-   0        0        0      371 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/specialbots/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/specialbots/_unlink.py
+-rw-rw-rw-   0        0        0    20247 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/specialbots/_upload.py
+-rw-rw-rw-   0        0        0    84825 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/textlib.py
+-rw-rw-rw-   0        0        0    12074 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/throttle.py
+-rw-rw-rw-   0        0        0    15061 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/time.py
+-rw-rw-rw-   0        0        0     3267 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/titletranslate.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.577140 pywikibot-8.1.1/pywikibot/tools/
+-rw-rw-rw-   0        0        0    27088 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/__init__.py
+-rw-rw-rw-   0        0        0    25467 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/_deprecate.py
+-rw-rw-rw-   0        0        0     1205 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/_logging.py
+-rw-rw-rw-   0        0        0    22207 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/_unidata.py
+-rw-rw-rw-   0        0        0     3116 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/chars.py
+-rw-rw-rw-   0        0        0     8765 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/collections.py
+-rw-rw-rw-   0        0        0    11075 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/djvu.py
+-rw-rw-rw-   0        0        0     4021 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/formatter.py
+-rw-rw-rw-   0        0        0     9745 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/itertools.py
+-rw-rw-rw-   0        0        0     7334 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/threading.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.587112 pywikibot-8.1.1/pywikibot/userinterfaces/
+-rw-rw-rw-   0        0        0      870 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/__init__.py
+-rw-rw-rw-   0        0        0     1906 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/_interface_base.py
+-rw-rw-rw-   0        0        0     2687 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/buffer_interface.py
+-rw-rw-rw-   0        0        0    22100 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/userinterfaces/gui.py
+-rw-rw-rw-   0        0        0      457 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/terminal_interface.py
+-rw-rw-rw-   0        0        0    24536 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/terminal_interface_base.py
+-rw-rw-rw-   0        0        0     2114 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/terminal_interface_unix.py
+-rw-rw-rw-   0        0        0     2012 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/terminal_interface_win32.py
+-rw-rw-rw-   0        0        0    90310 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/transliteration.py
+-rw-rw-rw-   0        0        0    16698 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/version.py
+-rw-rw-rw-   0        0        0     7366 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/xmlreader.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:50.995694 pywikibot-8.1.1/pywikibot.egg-info/
+-rw-rw-rw-   0        0        0    14586 2023-04-21 08:21:50.000000 pywikibot-8.1.1/pywikibot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10447 2023-04-21 08:21:50.000000 pywikibot-8.1.1/pywikibot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:21:50.000000 pywikibot-8.1.1/pywikibot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-21 08:21:50.000000 pywikibot-8.1.1/pywikibot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1228 2023-04-21 08:21:50.000000 pywikibot-8.1.1/pywikibot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-21 08:21:50.000000 pywikibot-8.1.1/pywikibot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 08:21:51.591101 pywikibot-8.1.1/setup.cfg
+-rw-rw-rw-   0        0        0    13116 2023-04-15 09:02:53.000000 pywikibot-8.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.588110 pywikibot-8.1.1/tests/
+-rw-rw-rw-   0        0        0     2814 2023-04-16 15:04:28.000000 pywikibot-8.1.1/tests/tests_tests.py
```

### Comparing `pywikibot-8.1.0/AUTHORS.rst` & `pywikibot-8.1.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/LICENSE` & `pywikibot-8.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/PKG-INFO` & `pywikibot-8.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 8.1.0
+Version: 8.1.1
 Summary: Python MediaWiki Bot Framework
 Home-page: https://www.mediawiki.org/wiki/Manual:Pywikibot
 Download-URL: https://pywikibot.toolforge.org/
 Maintainer: The Pywikibot team
 Maintainer-email: pywikibot@lists.wikimedia.org
 License: MIT License
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
@@ -257,32 +257,17 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* generate_family_filescript was improved (T334775)
-* A ``quiet`` parameter was added to APISite.preloadpages()
-  which is True by default
-* Fix getting HTTPStatus enum in site_detect check_response (T334728)
-* Do not show a logging in message if password is entered (T178061)
-* Enable preleading ``Bot:`` prefix with twtranslate messages (T161459)
-* Disable command.log if -nolog option is given (T334381)
-* Guess the last needed token key if the token is not found (T334288)
-* Show parameters with APIError (T333957)
-* Raise exceptions.NoSiteLinkErrorinstead of exceptions.NoPageErrorwhen sitelink
-  is missing in ItemPage.getSitelink()(T332341)
-* exceptions.ClientErrorwas added
-* Raise exceptions.NoPageErrorwhen deleting a missing Page (T332924)
-* ``text`` parameter of proofreadpage.PagesTagParserhas a default value
-* L10N updates
-* Ignore talk pages with APISite.watched_pages()(T330806)
-* Load page info when creating a page if not updated previously (T330980)
-* Improve flush exception logging
+* Add support for fatwikipedia (T335021)
+* Add support for kcgwiktionary (T334742)
+* Update for wowwiki family
 
 
 Deprecations
 ------------
 
 * 8.1.0: Dependency of exceptions.NoSiteLinkErrorfrom exceptions.NoPageErrorwill be removed
 * 8.1.0: ``exceptions.Server414Error`` is deprecated in favour of exceptions.Client414Error
```

### Comparing `pywikibot-8.1.0/README.rst` & `pywikibot-8.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/make_dist.py` & `pywikibot-8.1.1/make_dist.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/__init__.py` & `pywikibot-8.1.1/pywikibot/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/__metadata__.py` & `pywikibot-8.1.1/pywikibot/__metadata__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Distributed under the terms of the MIT license.
 #
 from time import strftime
 
 
 __name__ = 'pywikibot'
-__version__ = '8.1.0'
+__version__ = '8.1.1'
 __description__ = 'Python MediaWiki Bot Framework'
 __maintainer__ = 'The Pywikibot team'
 __maintainer_email__ = 'pywikibot@lists.wikimedia.org'
 __license__ = 'MIT License'
 __url__ = 'https://www.mediawiki.org/wiki/Manual:Pywikibot'
 __download_url__ = 'https://pywikibot.toolforge.org/'
 __copyright__ = '(C) Pywikibot team, 2003-' + strftime('%Y')
```

### Comparing `pywikibot-8.1.0/pywikibot/_wbtypes.py` & `pywikibot-8.1.1/pywikibot/_wbtypes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/backports.py` & `pywikibot-8.1.1/pywikibot/backports.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/bot.py` & `pywikibot-8.1.1/pywikibot/bot.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/bot_choice.py` & `pywikibot-8.1.1/pywikibot/bot_choice.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/comms/eventstreams.py` & `pywikibot-8.1.1/pywikibot/comms/eventstreams.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/comms/http.py` & `pywikibot-8.1.1/pywikibot/comms/http.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/config.py` & `pywikibot-8.1.1/pywikibot/config.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/cosmetic_changes.py` & `pywikibot-8.1.1/pywikibot/cosmetic_changes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/daemonize.py` & `pywikibot-8.1.1/pywikibot/daemonize.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/data/api/__init__.py` & `pywikibot-8.1.1/pywikibot/data/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/data/api/_generators.py` & `pywikibot-8.1.1/pywikibot/data/api/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/data/api/_optionset.py` & `pywikibot-8.1.1/pywikibot/data/api/_optionset.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/data/api/_paraminfo.py` & `pywikibot-8.1.1/pywikibot/data/api/_paraminfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/data/api/_requests.py` & `pywikibot-8.1.1/pywikibot/data/api/_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -936,15 +936,15 @@
         tokens = self.site.tokens.update_tokens(self._params['token'])
         self._params['token'] = tokens
         return True
 
     def submit(self) -> dict:
         """Submit a query and parse the response.
 
-        .. versionchanged:: 8.1
+        .. versionchanged:: 8.0.4
            in addition to *readapidenied* also try to login when API
            response is *notloggedin*.
 
         :return: a dict containing data retrieved from api.php
         """
         self._add_defaults()
         use_get = self._use_get()
```

### Comparing `pywikibot-8.1.0/pywikibot/data/memento.py` & `pywikibot-8.1.1/pywikibot/data/memento.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/data/mysql.py` & `pywikibot-8.1.1/pywikibot/data/mysql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/data/sparql.py` & `pywikibot-8.1.1/pywikibot/data/sparql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/data/wikistats.py` & `pywikibot-8.1.1/pywikibot/data/wikistats.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/date.py` & `pywikibot-8.1.1/pywikibot/date.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/diff.py` & `pywikibot-8.1.1/pywikibot/diff.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/echo.py` & `pywikibot-8.1.1/pywikibot/echo.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,14 @@
             notif.agent = None
 
         try:
             notif.read = pywikibot.Timestamp.fromtimestampformat(data['read'])
         except KeyError:
             notif.read = False
 
-        notif.content = data.get('*', None)
-        notif.revid = data.get('revid', None)
+        notif.content = data.get('*')
+        notif.revid = data.get('revid')
         return notif
 
     def mark_as_read(self) -> bool:
         """Mark the notification as read."""
         return self.site.notifications_mark_read(list=self.id)
```

### Comparing `pywikibot-8.1.0/pywikibot/editor.py` & `pywikibot-8.1.1/pywikibot/editor.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/exceptions.py` & `pywikibot-8.1.1/pywikibot/exceptions.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/families/commons_family.py` & `pywikibot-8.1.1/pywikibot/families/commons_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/families/lingualibre_family.py` & `pywikibot-8.1.1/pywikibot/families/lingualibre_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/families/meta_family.py` & `pywikibot-8.1.1/pywikibot/families/meta_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/families/osm_family.py` & `pywikibot-8.1.1/pywikibot/families/osm_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/families/vikidia_family.py` & `pywikibot-8.1.1/pywikibot/families/vikidia_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/families/wikibooks_family.py` & `pywikibot-8.1.1/pywikibot/families/wikibooks_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/families/wikidata_family.py` & `pywikibot-8.1.1/pywikibot/families/wikidata_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/families/wikihow_family.py` & `pywikibot-8.1.1/pywikibot/families/wikihow_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/families/wikimania_family.py` & `pywikibot-8.1.1/pywikibot/families/wikimania_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/families/wikimediachapter_family.py` & `pywikibot-8.1.1/pywikibot/families/wikimediachapter_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/families/wikinews_family.py` & `pywikibot-8.1.1/pywikibot/families/wikinews_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/families/wikipedia_family.py` & `pywikibot-8.1.1/pywikibot/families/wikipedia_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,42 +26,42 @@
     ]
 
     languages_by_size = [
         'en', 'ceb', 'de', 'sv', 'fr', 'nl', 'ru', 'es', 'it', 'arz', 'pl',
         'ja', 'zh', 'vi', 'war', 'uk', 'ar', 'pt', 'fa', 'ca', 'sr', 'id',
         'ko', 'no', 'ce', 'fi', 'hu', 'cs', 'tr', 'tt', 'sh', 'ro',
         'zh-min-nan', 'eu', 'ms', 'eo', 'he', 'hy', 'da', 'bg', 'cy', 'sk',
-        'azb', 'et', 'kk', 'be', 'simple', 'uz', 'min', 'el', 'hr', 'lt', 'gl',
+        'azb', 'uz', 'et', 'kk', 'be', 'simple', 'min', 'el', 'hr', 'lt', 'gl',
         'az', 'ur', 'sl', 'ka', 'nn', 'hi', 'th', 'ta', 'la', 'bn', 'mk',
         'ast', 'zh-yue', 'lld', 'lv', 'tg', 'af', 'my', 'mg', 'bs', 'mr', 'sq',
         'oc', 'nds', 'ml', 'be-tarask', 'te', 'ky', 'br', 'sw', 'jv', 'new',
         'vec', 'pnb', 'ht', 'pms', 'ba', 'lb', 'su', 'ku', 'ga', 'lmo', 'szl',
         'is', 'fy', 'cv', 'ckb', 'pa', 'tl', 'an', 'wuu', 'diq', 'io', 'sco',
         'vo', 'yo', 'ne', 'ia', 'gu', 'kn', 'als', 'avk', 'bar', 'scn', 'bpy',
         'ha', 'crh', 'qu', 'nv', 'mn', 'xmf', 'si', 'ban', 'ps', 'frr',
         'bat-smg', 'os', 'or', 'sah', 'cdo', 'gd', 'bug', 'yi', 'sd', 'ilo',
-        'am', 'nap', 'mzn', 'li', 'ig', 'gor', 'hsb', 'fo', 'map-bms', 'mai',
+        'am', 'nap', 'mzn', 'li', 'ig', 'gor', 'fo', 'hsb', 'map-bms', 'mai',
         'bcl', 'eml', 'shn', 'ace', 'zh-classical', 'sa', 'wa', 'as', 'ie',
-        'lij', 'zu', 'mhr', 'hyw', 'hif', 'mrj', 'sn', 'bjn', 'tum', 'mni',
+        'lij', 'zu', 'mhr', 'hyw', 'hif', 'sn', 'mrj', 'tum', 'bjn', 'mni',
         'km', 'hak', 'roa-tara', 'so', 'pam', 'rue', 'nso', 'bh', 'sat', 'se',
         'myv', 'mi', 'vls', 'nds-nl', 'nah', 'sc', 'kw', 'glk', 'vep', 'kab',
-        'tk', 'ary', 'gan', 'co', 'dag', 'fiu-vro', 'bo', 'ab', 'rw', 'gv',
+        'tk', 'ary', 'gan', 'dag', 'co', 'fiu-vro', 'bo', 'ab', 'rw', 'gv',
         'skr', 'ug', 'zea', 'frp', 'udm', 'pcd', 'kv', 'csb', 'mt', 'gn',
         'smn', 'ay', 'nrm', 'lez', 'lfn', 'olo', 'stq', 'mwl', 'lo', 'ang',
         'fur', 'rm', 'lad', 'gom', 'koi', 'ext', 'tyv', 'dsb', 'av', 'ln',
         'dty', 'kaa', 'pap', 'cbk-zam', 'dv', 'mdf', 'ksh', 'tw', 'ks', 'gag',
         'bxr', 'pfl', 'lg', 'za', 'pi', 'pag', 'szy', 'haw', 'awa', 'tay',
         'blk', 'inh', 'krc', 'xal', 'pdc', 'to', 'atj', 'arc', 'tcy', 'mnw',
         'jam', 'kbp', 'na', 'wo', 'kbd', 'nia', 'nov', 'shi', 'ki', 'nqo',
         'anp', 'bi', 'tpi', 'tet', 'jbo', 'roa-rup', 'xh', 'fj', 'om', 'kg',
         'lbe', 'ty', 'guw', 'cu', 'trv', 'srn', 'sm', 'alt', 'gcr', 'chr',
         'ltg', 'tn', 'ny', 'mad', 'st', 'pih', 'got', 'ee', 'rmy', 'ami', 'bm',
         'ff', 've', 'ts', 'chy', 'ss', 'kcg', 'rn', 'pcm', 'ch', 'ik', 'pnt',
-        'guc', 'ady', 'iu', 'ak', 'pwn', 'sg', 'din', 'ti', 'kl', 'dz', 'gur',
-        'cr',
+        'ady', 'guc', 'iu', 'ak', 'pwn', 'sg', 'din', 'ti', 'kl', 'dz', 'gur',
+        'fat', 'cr',
     ]
 
     # Sites we want to edit but not count as real languages
     test_codes = ['test', 'test2']
 
     # Templates that indicate a category redirect
     # Redirects to these templates are automatically included
```

### Comparing `pywikibot-8.1.0/pywikibot/families/wikiquote_family.py` & `pywikibot-8.1.1/pywikibot/families/wikiquote_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/families/wikisource_family.py` & `pywikibot-8.1.1/pywikibot/families/wikisource_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         'tokipona',
     ]
 
     languages_by_size = [
         'pl', 'en', 'ru', 'de', 'fr', 'zh', 'he', 'it', 'uk', 'ar', 'es',
         'mul', 'gu', 'cs', 'sr', 'pt', 'fa', 'sv', 'bn', 'hu', 'ko', 'ta',
         'ml', 'sa', 'te', 'sl', 'tr', 'vi', 'hy', 'la', 'el', 'ja', 'ro', 'fi',
-        'nl', 'nap', 'be', 'az', 'ca', 'hr', 'br', 'kn', 'no', 'id', 'th',
+        'nl', 'nap', 'be', 'az', 'ca', 'hr', 'br', 'kn', 'no', 'th', 'id',
         'eo', 'hi', 'is', 'vec', 'cy', 'ban', 'pms', 'mr', 'lij', 'da', 'et',
         'mk', 'as', 'yi', 'bg', 'jv', 'wa', 'li', 'lt', 'pa', 'or', 'eu', 'gl',
         'bs', 'sah', 'sk', 'zh-min-nan', 'fo',
     ]
 
     # Sites we want to edit but not count as real languages
     test_codes = ['beta']
```

### Comparing `pywikibot-8.1.0/pywikibot/families/wikiversity_family.py` & `pywikibot-8.1.1/pywikibot/families/wikiversity_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/families/wikivoyage_family.py` & `pywikibot-8.1.1/pywikibot/families/wikivoyage_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/families/wiktionary_family.py` & `pywikibot-8.1.1/pywikibot/families/wiktionary_family.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,18 @@
         'mnw', 'lo', 'simple', 'la', 'hr', 'sk', 'shn', 'fj', 'ky', 'wa', 'bg',
         'tg', 'ur', 'ps', 'cy', 'lmo', 'he', 'vo', 'om', 'sl', 'af',
         'zh-min-nan', 'scn', 'ms', 'tl', 'pa', 'fy', 'sw', 'ka', 'nn', 'min',
         'lv', 'sq', 'nds', 'gor', 'lb', 'co', 'mn', 'pnb', 'bs', 'nah', 'yue',
         'sa', 'kk', 'km', 'ckb', 'vec', 'be', 'diq', 'tk', 'mk', 'nia', 'sm',
         'hsb', 'ks', 'shy', 'su', 'bcl', 'gd', 'ga', 'an', 'gom', 'mr', 'wo',
         'mni', 'bjn', 'ia', 'ang', 'mt', 'fo', 'sd', 'tt', 'gn', 'so', 'ie',
-        'mi', 'csb', 'ha', 'ug', 'si', 'guw', 'st', 'hif', 'roa-rup', 'jbo',
-        'kl', 'zu', 'ay', 'yi', 'ln', 'gu', 'na', 'gv', 'kw', 'tpi', 'am',
-        'ne', 'rw', 'ts', 'ig', 'qu', 'ss', 'iu', 'chr', 'dv', 'ti', 'tn',
+        'ha', 'mi', 'csb', 'ug', 'si', 'guw', 'st', 'hif', 'roa-rup', 'jbo',
+        'kl', 'zu', 'ay', 'yi', 'ln', 'gu', 'na', 'gv', 'kw', 'tpi', 'kcg',
+        'am', 'ne', 'rw', 'ts', 'ig', 'qu', 'ss', 'iu', 'chr', 'dv', 'ti',
+        'tn',
     ]
 
     category_redirect_templates = {
         '_default': (),
         'ar': ('تحويل تصنيف',),
         'zh': ('分类重定向',),
     }
```

### Comparing `pywikibot-8.1.0/pywikibot/families/wowwiki_family.py` & `pywikibot-8.1.1/pywikibot/families/wowwiki_family.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Family module for WOW wiki."""
 #
-# (C) Pywikibot team, 2009-2022
+# (C) Pywikibot team, 2009-2023
 #
 # Distributed under the terms of the MIT license.
 #
 from pywikibot import family
 from pywikibot.tools import classproperty
 
 
@@ -13,30 +13,29 @@
     """Family class for WOW Wiki."""
 
     name = 'wowwiki'
     domain = 'wowwiki.fandom.com'
 
     codes = (
         'ar', 'cs', 'da', 'de', 'el', 'en', 'es', 'et', 'fa', 'fi', 'fr', 'he',
-        'hu', 'is', 'it', 'ja', 'ko', 'lt', 'lv', 'nl', 'no', 'pl', 'pt',
-        'pt-br', 'ru', 'sk', 'sv', 'tr', 'uk', 'zh', 'zh-tw'
+        'hu', 'it', 'ja', 'ko', 'nl', 'no', 'pl', 'pt', 'pt-br', 'ru', 'uk',
+        'zh', 'zh-tw',
     )
 
-    removed_wikis = ['hr', 'ro', 'sr']
+    removed_wikis = ['is', 'hr', 'lt', 'lv', 'ro', 'sk', 'sr', 'sv', 'tr']
 
     code_aliases = {'nn': 'no'}
 
     @classproperty
     def langs(cls):
         """Property listing family languages."""
         cls.langs = super().langs
         # override deviations
-        for i, lang in enumerate(['es', 'et', 'sv'], start=1):
+        for i, lang in enumerate(['en', 'es', 'et', 'uk'], start=1):
             cls.langs[lang] = cls.domains[i]
-        cls.langs['uk'] = cls.domains[-1]
         return cls.langs
 
     @classproperty
     def disambiguationTemplates(cls):  # noqa: N802
         """Property listing disambiguation templates."""
         cls.disambiguationTemplates = super().disambiguationTemplates
         cls.disambiguationTemplates['en'] = ['disambig', 'disambig/quest',
@@ -57,16 +56,17 @@
         """Property listing site keys for categories at last position."""
         return cls.langs.keys()
 
     @classproperty
     def domains(cls):
         """List of domains used by family wowwiki."""
         return [cls.domain,
-                'wow-es.gamepedia.com',  # es
+                'wowwiki-archive.fandom.com',  # en
+                'wow.gamepedia.com',  # es
                 'worldofwarcraft.fandom.com',  # et
-                'warcraft.fandom.com']  # sv, uk
+                'warcraft.fandom.com']  # uk
 
     def scriptpath(self, code):
         """Return the script path for this family."""
         if code == 'es':
             return ''
         return super().scriptpath(code)
```

### Comparing `pywikibot-8.1.0/pywikibot/family.py` & `pywikibot-8.1.1/pywikibot/family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/fixes.py` & `pywikibot-8.1.1/pywikibot/fixes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/flow.py` & `pywikibot-8.1.1/pywikibot/flow.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/i18n.py` & `pywikibot-8.1.1/pywikibot/i18n.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/interwiki_graph.py` & `pywikibot-8.1.1/pywikibot/interwiki_graph.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/logentries.py` & `pywikibot-8.1.1/pywikibot/logentries.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/logging.py` & `pywikibot-8.1.1/pywikibot/logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/login.py` & `pywikibot-8.1.1/pywikibot/login.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/page/__init__.py` & `pywikibot-8.1.1/pywikibot/page/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/page/_basepage.py` & `pywikibot-8.1.1/pywikibot/page/_basepage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/page/_category.py` & `pywikibot-8.1.1/pywikibot/page/_category.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/page/_collections.py` & `pywikibot-8.1.1/pywikibot/page/_collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/page/_decorators.py` & `pywikibot-8.1.1/pywikibot/page/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/page/_filepage.py` & `pywikibot-8.1.1/pywikibot/page/_filepage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/page/_links.py` & `pywikibot-8.1.1/pywikibot/page/_links.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/page/_page.py` & `pywikibot-8.1.1/pywikibot/page/_page.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/page/_revision.py` & `pywikibot-8.1.1/pywikibot/page/_revision.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/page/_toolforge.py` & `pywikibot-8.1.1/pywikibot/page/_toolforge.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/page/_user.py` & `pywikibot-8.1.1/pywikibot/page/_user.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/page/_wikibase.py` & `pywikibot-8.1.1/pywikibot/page/_wikibase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1575,15 +1575,15 @@
         :param data: JSON containing claim data
         :type data: dict
 
         :rtype: pywikibot.page.Claim
         """
         claim_repo = site.get_repo_for_entity_type('property')
         claim = cls(claim_repo, data['mainsnak']['property'],
-                    datatype=data['mainsnak'].get('datatype', None))
+                    datatype=data['mainsnak'].get('datatype'))
         if 'id' in data:
             claim.snak = data['id']
         elif 'hash' in data:
             claim.hash = data['hash']
         claim.snaktype = data['mainsnak']['snaktype']
         if claim.getSnakType() == 'value':
             value = data['mainsnak']['datavalue']['value']
```

### Comparing `pywikibot-8.1.0/pywikibot/pagegenerators/__init__.py` & `pywikibot-8.1.1/pywikibot/pagegenerators/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/pagegenerators/_factory.py` & `pywikibot-8.1.1/pywikibot/pagegenerators/_factory.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/pagegenerators/_filters.py` & `pywikibot-8.1.1/pywikibot/pagegenerators/_filters.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/pagegenerators/_generators.py` & `pywikibot-8.1.1/pywikibot/pagegenerators/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/plural.py` & `pywikibot-8.1.1/pywikibot/plural.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/proofreadpage.py` & `pywikibot-8.1.1/pywikibot/proofreadpage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/__init__.py` & `pywikibot-8.1.1/pywikibot/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/generate_family_file.py` & `pywikibot-8.1.1/pywikibot/scripts/generate_family_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
                 if not pywikibot.bot.input_yn(
                     'Retry with disabled ssl certificate validation',
                     default=self.verify, automatic_quit=False,
                         force=self.verify is not None):
                     break
             else:
                 return w, verify
-        return None, None
+        return None, None  # pragma: no cover
 
     def run(self) -> None:
         """Main method, generate family file."""
         if not self.get_params():
             return
 
         w, verify = self.get_wiki()
@@ -178,15 +178,15 @@
                                'local': '',
                                'prefix': w.lang,
                                'url': w.iwpath})
 
         code_len = len(self.langs)
         if code_len > 1:
             if self.dointerwiki is None:
-                while True:
+                while True:  # pragma: no cover
                     makeiw = input(
                         '\n'
                         f'There are {code_len} sites available.'
                         ' Do you want to generate interwiki links?\n'
                         'This might take a long time. '
                         '([y]es, [s]trict, [N]o, [e]dit), [h]elp) ').lower()
                     if makeiw in ('y', 's', 'n', 'e', ''):
@@ -206,15 +206,15 @@
                 self.langs = [wiki for wiki in self.langs
                               if wiki['url'] == w.iwpath]
             elif makeiw == 's':
                 domain = '.'.join(urlparse(w.server).hostname.split('.')[1:])
                 self.langs = [wiki for wiki in self.langs
                               if domain in wiki['url']]
 
-            elif makeiw == 'e':
+            elif makeiw == 'e':  # pragma: no cover
                 for wiki in self.langs:
                     print(wiki['prefix'], wiki['url'])
                 do_langs = re.split(' *,| +',
                                     input('Which sites do you want: '))
                 self.langs = [wiki for wiki in self.langs
                               if wiki['prefix'] in do_langs
                               or wiki['url'] == w.iwpath]
```

### Comparing `pywikibot-8.1.0/pywikibot/scripts/generate_user_files.py` & `pywikibot-8.1.1/pywikibot/scripts/generate_user_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,28 +309,28 @@
     # First ask what to do which the whole section type variant
     select = 'h'
     answers = [('Yes', 'y'), ('All', 'a'), ('None', 'n'), ('Help', 'h')]
     while select == 'h':
         select = pywikibot.input_choice(
             f'Do you want to select {variant} setting sections?',
             answers, default=default, force=force, automatic_quit=False)
-        if select == 'h':
+        if select == 'h':  # pragma: no cover
             answers.pop(-1)
             pywikibot.info(
                 f'The following {variant} setting sections are provided:')
             for item in filter(skip, sections):
                 pywikibot.info(item.head)
 
     copies = []
     # Now ask for a single section of the given variant
     # or use all or none of them
     choice = {'a': 'all', 'n': 'none', 'y': 'h'}[select]  # mapping
     for item in filter(skip, sections):
         answers = [('Yes', 'y'), ('No', 'n'), ('Help', 'h')]
-        while choice == 'h':
+        while choice == 'h':  # pragma: no cover
             choice = pywikibot.input_choice(
                 f'Do you want to add {item.head} section?',
                 answers, default='n', force=force, automatic_quit=False)
             if choice == 'h':
                 answers.pop(-1)
                 pywikibot.info(fill(item.info))
         if choice in ('all', 'y'):
```

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ar.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ar.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ast.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ast.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/az.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/az.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/azb.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/azb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ba.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ba.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bcc.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bcc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/be-tarask.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/be-tarask.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/be.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/be.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bg.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bn.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/br.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bs.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ca.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ca.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ce.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ce.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ckb.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ckb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/cs.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/cs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/csb.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/csb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/cy.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/cy.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/da.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/da.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/de.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/de.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/diq.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/diq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/el.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/el.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/en.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/en.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/eo.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/eo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/es.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/es.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/eu.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/eu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fa.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fa.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fi.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fo.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fr.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/frr.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/frr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/gl.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/gl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/gsw.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/gsw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hak.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hak.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/haw.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/haw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/he.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/he.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hi.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hsb.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hsb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hu.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ia.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ia.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/id.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/id.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/io.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/io.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/is.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/is.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/it.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/it.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ja.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ja.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/kab.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/kab.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/kk.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/kk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/km.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/km.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/kn.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/kn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ko.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ko.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/krc.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/krc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ksh.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ksh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/lb.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/lb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/lt.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/lt.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/lv.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/lv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/map-bms.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/map-bms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/mg.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/mg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/min.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/min.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/mk.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/mk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ml.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ml.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ms.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/my.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/my.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nan.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nan.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nb.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nds-nl.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nds-nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ne.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ne.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/new.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/new.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nl.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nqo.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nqo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pl.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pms.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pt-br.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pt-br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pt.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pt.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/qqq.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/qqq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ro.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ro.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ru.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ru.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sco.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sco.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sh.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/si.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/si.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sk.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sl.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/so.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/so.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sr.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sv.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sw.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ta.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ta.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/te.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/te.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/th.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/th.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tly.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tly.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tr.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/uk.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/uk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ur.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ur.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/vi.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/vi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/yue.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/yue.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/zh.json` & `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/zh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/login.py` & `pywikibot-8.1.1/pywikibot/scripts/login.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/preload_sites.py` & `pywikibot-8.1.1/pywikibot/scripts/preload_sites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/shell.py` & `pywikibot-8.1.1/pywikibot/scripts/shell.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/version.py` & `pywikibot-8.1.1/pywikibot/scripts/version.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/scripts/wrapper.py` & `pywikibot-8.1.1/pywikibot/scripts/wrapper.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/site/__init__.py` & `pywikibot-8.1.1/pywikibot/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/site/_apisite.py` & `pywikibot-8.1.1/pywikibot/site/_apisite.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,17 +328,17 @@
         autocreate: bool = False,
         user: Optional[str] = None,
         *,
         cookie_only: bool = False
     ) -> None:
         """Log the user in if not already logged in.
 
-        .. versionchanged:: 8.0
-           lazy load cookies when logging in. This was dropped in 8.1
-        .. versionchanged:: 8.1
+        .. versionchanged:: 8.0.0
+           lazy load cookies when logging in. This was dropped in 8.0.4
+        .. versionchanged:: 8.0.4
            the *cookie_only* parameter was added and cookies are loaded
            whenever the site is initialized.
 
         .. seealso:: :api:`Login`
 
         :param autocreate: if true, allow auto-creation of the account
             using unified login
```

### Comparing `pywikibot-8.1.0/pywikibot/site/_basesite.py` & `pywikibot-8.1.1/pywikibot/site/_basesite.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,12 +410,12 @@
     def category_on_one_line(self):
         # TODO: is this even needed? No family in the framework uses it.
         """Return True if this site wants all category links on one line."""
         return self.code in self.family.category_on_one_line
 
     def interwiki_putfirst(self):
         """Return list of language codes for ordering of interwiki links."""
-        return self.family.interwiki_putfirst.get(self.code, None)
+        return self.family.interwiki_putfirst.get(self.code)
 
     def getSite(self, code):  # noqa: N802
         """Return Site object for language 'code' in this Family."""
         return pywikibot.Site(code=code, fam=self.family, user=self.user())
```

### Comparing `pywikibot-8.1.0/pywikibot/site/_datasite.py` & `pywikibot-8.1.1/pywikibot/site/_datasite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/site/_decorators.py` & `pywikibot-8.1.1/pywikibot/site/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/site/_extensions.py` & `pywikibot-8.1.1/pywikibot/site/_extensions.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/site/_generators.py` & `pywikibot-8.1.1/pywikibot/site/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/site/_interwikimap.py` & `pywikibot-8.1.1/pywikibot/site/_interwikimap.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/site/_namespace.py` & `pywikibot-8.1.1/pywikibot/site/_namespace.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/site/_obsoletesites.py` & `pywikibot-8.1.1/pywikibot/site/_obsoletesites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/site/_siteinfo.py` & `pywikibot-8.1.1/pywikibot/site/_siteinfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/site/_tokenwallet.py` & `pywikibot-8.1.1/pywikibot/site/_tokenwallet.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/site/_upload.py` & `pywikibot-8.1.1/pywikibot/site/_upload.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/site_detect.py` & `pywikibot-8.1.1/pywikibot/site_detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,32 +89,33 @@
                 if self.api != self.fromurl and self.private_wiki:
                     self.articlepath = self.fromurl.rsplit('/', 1)[0] + '/$1'
                 else:
                     raise RuntimeError(
                         'Unable to determine articlepath because the wiki is '
                         'private. Use the Main Page URL instead of the API.')
             else:
-                raise RuntimeError('Unable to determine articlepath: '
-                                   '{}'.format(self.fromurl))
+                raise RuntimeError(
+                    f'Unable to determine articlepath: {self.fromurl}')
 
     def __repr__(self) -> str:
-        return '{}("{}")'.format(
-            self.__class__.__name__, self.fromurl)
+        return f'{type(self).__name__}("{self.fromurl}")'
 
     @property
     def langs(self):
         """Build interwikimap."""
         response = fetch(
             self.api
             + '?action=query&meta=siteinfo&siprop=interwikimap'
               '&sifilteriw=local&format=json')
         iw = response.json()
-        if 'error' in iw:
-            raise RuntimeError('{} - {}'.format(iw['error']['code'],
-                                                iw['error']['info']))
+
+        error = iw.get('error')
+        if error:
+            raise RuntimeError(f"{error['code']} - {error['info']}")
+
         return [wiki for wiki in iw['query']['interwikimap']
                 if 'language' in wiki]
 
     def _fetch_old_version(self) -> None:
         """Extract the version from API help with ?version enabled."""
         if self.version is None:
             try:
@@ -147,17 +148,16 @@
             # user config is not loaded because PYWIKIBOT_NO_USER_CONFIG
             # is set to '2' by generate_family_file.py.
             # Prepare a temporary config for login.
             username = pywikibot.input(
                 'Private wiki detected. Login is required.\n'
                 'Please enter your username?')
             # Setup a dummy family so that we can create a site object
-            fam = pywikibot.family.AutoFamily(
-                'temporary_family',
-                self.api[:-8])
+            fam = pywikibot.family.AutoFamily('temporary_family',
+                                              self.server + self.scriptpath)
             site = pywikibot.Site(fam.code, fam, username)
             site.version = lambda: str(self.version)
             # Now the site object is able to login
             info = site.siteinfo
         else:
             info = info['query']['general']
 
@@ -255,16 +255,16 @@
                         or self._parsed_url.netloc in new_parsed_url.netloc):
                     return
 
                 assert new_parsed_url == self._parsed_url, '{} != {}'.format(
                     self._parsed_url, new_parsed_url)
 
         self._parsed_url = new_parsed_url
-        self.server = '{}://{}'.format(
-            self._parsed_url.scheme, self._parsed_url.netloc)
+        self.server = '{url.scheme}://{url.netloc}'.format(
+            url=self._parsed_url)
         self.scriptpath = self._parsed_url.path
 
     def handle_starttag(self, tag, attrs) -> None:
         """Handle an opening tag."""
         attrs = dict(attrs)
         if tag == 'meta':
             if attrs.get('name') == 'generator':
```

### Comparing `pywikibot-8.1.0/pywikibot/specialbots/_unlink.py` & `pywikibot-8.1.1/pywikibot/specialbots/_unlink.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/specialbots/_upload.py` & `pywikibot-8.1.1/pywikibot/specialbots/_upload.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/textlib.py` & `pywikibot-8.1.1/pywikibot/textlib.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/throttle.py` & `pywikibot-8.1.1/pywikibot/throttle.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/time.py` & `pywikibot-8.1.1/pywikibot/time.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/titletranslate.py` & `pywikibot-8.1.1/pywikibot/titletranslate.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/tools/__init__.py` & `pywikibot-8.1.1/pywikibot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/tools/_deprecate.py` & `pywikibot-8.1.1/pywikibot/tools/_deprecate.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/tools/_logging.py` & `pywikibot-8.1.1/pywikibot/tools/_logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/tools/_unidata.py` & `pywikibot-8.1.1/pywikibot/tools/_unidata.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/tools/chars.py` & `pywikibot-8.1.1/pywikibot/tools/chars.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/tools/collections.py` & `pywikibot-8.1.1/pywikibot/tools/collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/tools/djvu.py` & `pywikibot-8.1.1/pywikibot/tools/djvu.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/tools/formatter.py` & `pywikibot-8.1.1/pywikibot/tools/formatter.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/tools/itertools.py` & `pywikibot-8.1.1/pywikibot/tools/itertools.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/tools/threading.py` & `pywikibot-8.1.1/pywikibot/tools/threading.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/userinterfaces/__init__.py` & `pywikibot-8.1.1/pywikibot/userinterfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/userinterfaces/_interface_base.py` & `pywikibot-8.1.1/pywikibot/userinterfaces/_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/userinterfaces/buffer_interface.py` & `pywikibot-8.1.1/pywikibot/userinterfaces/buffer_interface.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/userinterfaces/gui.py` & `pywikibot-8.1.1/pywikibot/userinterfaces/gui.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/userinterfaces/terminal_interface_base.py` & `pywikibot-8.1.1/pywikibot/userinterfaces/terminal_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/userinterfaces/terminal_interface_unix.py` & `pywikibot-8.1.1/pywikibot/userinterfaces/terminal_interface_unix.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/userinterfaces/terminal_interface_win32.py` & `pywikibot-8.1.1/pywikibot/userinterfaces/terminal_interface_win32.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/userinterfaces/transliteration.py` & `pywikibot-8.1.1/pywikibot/userinterfaces/transliteration.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/version.py` & `pywikibot-8.1.1/pywikibot/version.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot/xmlreader.py` & `pywikibot-8.1.1/pywikibot/xmlreader.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot.egg-info/PKG-INFO` & `pywikibot-8.1.1/pywikibot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 8.1.0
+Version: 8.1.1
 Summary: Python MediaWiki Bot Framework
 Home-page: https://www.mediawiki.org/wiki/Manual:Pywikibot
 Download-URL: https://pywikibot.toolforge.org/
 Maintainer: The Pywikibot team
 Maintainer-email: pywikibot@lists.wikimedia.org
 License: MIT License
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
@@ -257,32 +257,17 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* generate_family_filescript was improved (T334775)
-* A ``quiet`` parameter was added to APISite.preloadpages()
-  which is True by default
-* Fix getting HTTPStatus enum in site_detect check_response (T334728)
-* Do not show a logging in message if password is entered (T178061)
-* Enable preleading ``Bot:`` prefix with twtranslate messages (T161459)
-* Disable command.log if -nolog option is given (T334381)
-* Guess the last needed token key if the token is not found (T334288)
-* Show parameters with APIError (T333957)
-* Raise exceptions.NoSiteLinkErrorinstead of exceptions.NoPageErrorwhen sitelink
-  is missing in ItemPage.getSitelink()(T332341)
-* exceptions.ClientErrorwas added
-* Raise exceptions.NoPageErrorwhen deleting a missing Page (T332924)
-* ``text`` parameter of proofreadpage.PagesTagParserhas a default value
-* L10N updates
-* Ignore talk pages with APISite.watched_pages()(T330806)
-* Load page info when creating a page if not updated previously (T330980)
-* Improve flush exception logging
+* Add support for fatwikipedia (T335021)
+* Add support for kcgwiktionary (T334742)
+* Update for wowwiki family
 
 
 Deprecations
 ------------
 
 * 8.1.0: Dependency of exceptions.NoSiteLinkErrorfrom exceptions.NoPageErrorwill be removed
 * 8.1.0: ``exceptions.Server414Error`` is deprecated in favour of exceptions.Client414Error
```

### Comparing `pywikibot-8.1.0/pywikibot.egg-info/SOURCES.txt` & `pywikibot-8.1.1/pywikibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/pywikibot.egg-info/requires.txt` & `pywikibot-8.1.1/pywikibot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/setup.py` & `pywikibot-8.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.0/tests/tests_tests.py` & `pywikibot-8.1.1/tests/tests_tests.py`

 * *Files identical despite different names*

