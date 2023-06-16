<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

Inapendekezwa kusakinisha nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) kwanza, na kisha `direnv allow` baada ya kuingia saraka ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) itatekelezwa moja kwa moja baada ya kuingia saraka).

Maana ni: Tafsiri ya Kichina kwa Kijapani, Kikorea, Kiingereza, tafsiri ya Kiingereza kwa lugha zingine zote. Ikiwa ungependa kuunga mkono Kichina na Kiingereza pekee, unaweza kuandika `zh: en` .

Maana ni: Tafsiri ya Kichina kwa Kijapani, Kikorea, Kiingereza, tafsiri ya Kiingereza kwa lugha zingine zote. Ikiwa ungependa kuunga mkono Kichina na Kiingereza pekee, unaweza kuandika `zh: en` .

* [nambari ya mbele](https://github.com/xxai-art/web)
* [Pakiti za lugha kwa tovuti kwa ujumla](https://github.com/xxai-art/web/tree/main/i18n)
* [Pakiti za lugha za moduli za kuingia](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [Hati za Tovuti kwa Lugha nyingi](https://github.com/xxai-doc)

Lugha ya programu ya mwisho ni [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) , ambayo huongeza baadhi ya vipengele kulingana na sintaksia ya hati ya kahawa, angalia [./coffee_plus.md](./coffee_plus.md) .

## Kimataifa ya tovuti na nyaraka

Jenga kwenye miradi 3 ifuatayo

* [@w5/mdt](https://www.npmjs.com/package/@w5/mdt)

  Kiambishi tamati ni `.mdt` , unaweza kutumia sintaksia sawa na `<+ ./coffee_plus/import.js>` kurejelea faili za nje, na kutoa alama kwa kiambishi tamati `.md` .

* [@w5/trmd](https://www.npmjs.com/package/@w5/trmd)

  Tafsiri ya Markdown haitatafsiri misimbo na viungo, na itahifadhi sentensi zilizotafsiriwa. Ikiwa tafsiri itarekebishwa lakini maandishi asilia hayajarekebishwa, kuitekeleza tena hakutabatilisha urekebishaji wa tafsiri.

* [@w5/i18n](https://www.npmjs.com/package/@w5/i18n)

  Faili za lugha za kutafsiri tovuti zinazozalishwa na `yaml` .

### Maagizo ya Kiotomatiki ya Tafsiri ya Hati

Tazama hazina ya msimbo [xxai-art/doc](https://github.com/xxai-art/doc)

Inapendekezwa kusakinisha nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) kwanza, na kisha `direnv allow` baada ya kuingia saraka ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) itatekelezwa moja kwa moja baada ya kuingia saraka).

Ili kuepuka msingi mkubwa wa msimbo uliotafsiriwa katika mamia ya lugha, niliunda msingi tofauti wa msimbo kwa kila lugha na kuunda shirika la kuhifadhi msingi wa msimbo.

Kuweka utofauti wa mazingira `GITHUB_ACCESS_TOKEN` na kisha kuendesha [create.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) kutaunda hazina ya msimbo kiotomatiki.

Bila shaka, unaweza pia kuiweka katika msingi wa kanuni.

Rejeleo la hati ya tafsiri [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

Nambari ya maandishi inatafsiriwa kama ifuatavyo:

[bunx](https://bun.sh/docs/cli/bunx) ni badala ya npx, ambayo ni haraka zaidi. Bila shaka, ikiwa huna bun iliyosakinishwa, unaweza kutumia `npx` badala yake.

`bunx mdt zh` renders `.mdt` katika saraka ya zh kama `.md` , angalia faili 2 zilizounganishwa hapa chini

* [kahawa_plus.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [kahawa_plus.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` ndio msimbo wa msingi wa tafsiri (ikiwa una `nodejs` pekee zilizosakinishwa, lakini `bun` na `direnv` hazijasakinishwa, unaweza pia kuendesha `npx i18n` kutafsiri).

Itachanganua [i18n.yml](https://github.com/xxai-art/doc/blob/main/i18n.yml) , usanidi wa `i18n.yml` katika hati hii ni kama ifuatavyo:

```
en:
zh: ja ko en
```

Maana ni: Tafsiri ya Kichina kwa Kijapani, Kikorea, Kiingereza, tafsiri ya Kiingereza kwa lugha zingine zote. Ikiwa ungependa kuunga mkono Kichina na Kiingereza pekee, unaweza kuandika `zh: en` .

Ya mwisho ni [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) , ambayo hutoa maudhui kati ya kichwa kikuu na manukuu ya kwanza ya `README.md` ya kila lugha ili kutoa ingizo `README.md` . Kanuni ni rahisi sana, unaweza kuiangalia mwenyewe.

API ya Google inatumika kwa tafsiri isiyolipishwa. Ikiwa huwezi kufikia Google, tafadhali sanidi na uweke seva mbadala, kama vile:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

Hati ya tafsiri itazalisha akiba iliyotafsiriwa katika saraka `.i18n` , tafadhali iangalie na `git status` na uiongeze kwenye hazina ya msimbo ili kuepuka tafsiri zinazorudiwa.

Tafadhali endesha `bunx i18n` kila wakati unaporekebisha tafsiri ili kusasisha akiba.

Ikiwa maandishi ya asili na tafsiri yanarekebishwa kwa wakati mmoja, cache itachanganyikiwa, kwa hivyo ikiwa unataka kurekebisha, unaweza kurekebisha moja tu, na kisha kukimbia `bunx i18n` ili kusasisha cache.
