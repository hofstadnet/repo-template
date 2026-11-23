# <repo-navn>

<!-- Én setning: hva repoet er, og for hvem. -->

## Kom i gang

<!-- Hvordan installere, bygge og teste lokalt. -->

## Etter at repoet er laget fra malen

- [ ] Fyll inn denne README-en og `description` på repoet.
- [ ] Fyll inn `AGENTS.md`: prosjektet, kommandoene og reglene som gjelder repoet. Felles regler:
      https://github.com/hofstadnet/guidelines.
- [ ] `.github/workflows/code-scanning.yml`: legg til språkene repoet bruker.
- [ ] `.github/dependabot.yml`: slå på økosystemene repoet bruker.
- [ ] `.github/workflows/dependabot-automerge.yml`: utvid til flere økosystemer når repoet har tester som fanger
      brudd, og bruk et app-token hvis repoet publiserer ved push til `main`.
- [ ] Privat repo: slett `.github/workflows/scorecard.yml`.
- [ ] Legg repoet til i `github.json` i [hofstadnet/operations](https://github.com/hofstadnet/operations) (synlighet,
      beskrivelse og påkrevde sjekker) i en pull request, og kjør `node scripts/apply-settings.mjs --repo <navn>` og så
      `--apply` der når den er merget. Det setter regelsettet, sikkerhetsinnstillingene og tilgangen for teamet, som
      ikke følger med når et repo lages fra en mal. Et repo som ikke står i `github.json`, meldes av den ukentlige
      kontrollen.
- [ ] Legg til en `build`/`test`-jobb og legg den til som påkrevd sjekk i `github.json`.

## Sikkerhet

Se [SECURITY.md](SECURITY.md).
