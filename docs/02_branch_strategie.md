# Branch-Strategie

## Übersicht

In diesem Projekt verwenden wir eine einfache Feature-Branch-Strategie, die auf dem GitHub Flow basiert. Der `main`-Branch enthält immer den stabilen, produktionsreifen Code.

## Branches

| Branch | Zweck |
|--------|-------|
| `main` | Stabiler Hauptbranch, nur via Pull Request befüllbar |
| `feat/*` | Neue Features oder Aufgaben |
| `fix/*` | Bugfixes und kleine Korrekturen |
| `docs/*` | Reine Dokumentationsänderungen |

## Workflow

1. Neuen Branch von `main` erstellen: `git checkout -b feat/MeinFeature`
2. Änderungen committen (Conventional Commits)
3. Branch auf GitHub pushen
4. Pull Request erstellen und reviewen
5. Nach Genehmigung in `main` mergen
6. Branch löschen

## Commit-Konventionen

Wir nutzen [Conventional Commits](https://www.conventionalcommits.org/ ):

- `feat:` – Neues Feature
- `fix:` – Bugfix
- `docs:` – Dokumentation
- `ci:` – CI/CD Änderungen
- `chore:` – Sonstige Wartungsarbeiten

## Branch-Protection

Der `main`-Branch ist geschützt:
- Direktes Pushen ist nicht erlaubt
- Änderungen nur via Pull Request
- Mindestens 1 Review erforderlich (empfohlen)
