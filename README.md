# Gitkurs - tentative notater

Slides: [gitkurs.pdf](https://github.com/kaprests/Gitkurs/blob/master/gitkurs.pdf)

- Hva er Git?
    - Git != Github
    - versjonskontroll
- Oversikt over terminologi
    - Commit
    - Branch
    - Repository
        - local/remote (github)
- Commits: "Snapshot"
    - kul illustrasjon
    - Består av
        - Endring
        - parent
        - hash code
    - Kan alltid returnere til tidligere commits
- Branches
    - Kanskje senere??
    - Alle commits tilhører en branch
    - hovedbranch: master (som regel)
    - Head: ref. til nåværende branch
    - Illustrasjon her
    - Hvorfor branching?
    - Merging
    - Merge conflicts
- Repository (repo)
    - Inneholder:
        - Alle filer du vil holde styr på og deres endringshistorikk
        - Alle commits
    - Remote repository: i.e. GitHub
        - cloning
        - pull/push
        - Kommer tilbake til dette
- Hvordan bruke Git
    - kommandolinje
        - Finnes grafiske verktøy :((
        - For windowsfolk:
            - Gitbash?
            - annet???
            - subsystem?
            - Linux ;))
    - Oversikt over kommandoer (rekkefølge) -- Illustrasjoner, lastebil ellerno
        - git init (initiere git repo)
        - lokalt repo
            - * gjøre endringer*
            - git add <filnavn> (staging)
                stage alt: git add -A
            - git commit
        - med remote, kun deg
            - * gjøre endringer*
            - git add
            - git commit
            - git push
        - flere bidragsytere, liten endring
            - * gjøre endringer*
            - git add
            - git commit
            - git pull
            - git push
        - flere bidragsytere, større endring
            - git branh <min nye branch>
            - git checkout <min nye branch>
            - * gjøre endringer*
            - git add x 5
            - git commit x 5
            - git checkout master
            - git pull
            - git merge <min nye branch>
            - git push
- Oppgaver
    - Opprett git repository:
        - lag prosjektmappe (ev. bruk noe du har fra før)
        - git init
    - Opprett noen commits
        - gjør endringer (legge til fil, endre fil, slette fil etc.)
        - stage ønskede endringer (git add <filnavn>)
        - commit (git commit)
        - Gjenta noen ganger
    - Få det på GitHub!
        - Opprett nytt, tomt repo på GitHub
        - set remote
        - push til GitHub (git push (set origin...))
    - Bidra på eksisterende prosjekt
        - klon repoet vårt (git clone...)
        - lag branch (git branch...)
            - git checkout <branch>
        - endringer, stage, commit
        - merge din branch inn i master
            - Bytt til master (git checkout master)
            - Hent nyeste endringer fra origin/master (git pull)
            - Merge (git merge <din branch med kule endringer>)
                - Løs eventuelle konflikter
            - Oppdater origin (GitHub) (git push)
- Om du kan å gjøre alt dette er du nok på nivå med den gjengse WebKommer! :))








