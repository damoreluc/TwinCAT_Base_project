# Progetto base TwinCAT3 con gestione versionamento
Progetto di base per TwinCAT3 da utilizare come template per nuovi progetti da gestire tramite Git e GitHub

## Istruzioni per l'uso
1. iniziare una sessione su GitHub
2. creare un *nuovo repository* con le opzioni seguenti:
    1. nel campo **Repository template** selezionare l'opzione **damoreluc/TwinCAT_Base_project**
    2. nel campo **Repository name** scegliere il nome del nuovo progetto, ad esempio `TwinCAT_dal_base_project`
    3. nel campo **Description** specificare, se voluto, una descrizione sintetica del nuovo progetto
    4. selezionare la visibilità del nuovo repository con l'opzione _Public_ o _Private_
    5. completare la creazione del nuovo repository premendo il pulsante **Create repository**
3. Passare alla pagina `<>Code` del nuovo repository
4. Clic sul pulsante verde `<>Code` e copiare l'indirizzo del nuovo repository da clonare localmente, ad esempio `https://github.com/damoreluc/TwinCAT_dal_base_project.git`
5. nel ***proprio PC***, aprire la cartella principale dei progetti TwinCAT, di solito è `Documenti\TcXaeShell`
6. da qui avviare un terminale di Windows col comando `clic destro -> Apri nel terminale`
7. clonare il repository digitando nel terminale il comando 
   > `git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY`

   come esempio:

   `git clone https://github.com/damoreluc/TwinCAT_dal_base_project.git`

   si dovrebbero ottenere messaggi simili ai seguenti:
   ```
   remote: Enumerating objects: 18, done.
   remote: Counting objects: 100% (18/18), done.
   remote: Compressing objects: 100% (15/15), done.
   remote: Total 18 (delta 1), reused 13 (delta 0), pack-reused 0
   Receiving objects: 100% (18/18), 8.72 KiB | 2.91 MiB/s, done.
   Resolving deltas: 100% (1/1), done.
   ```
   
   il repository remoto verrà clonato localmente in una nuova cartella con lo stesso nome del repository remoto, dentro il percorso principale dei progetti TwinCAT `Documenti\TcXaeShell`

9. *opzionale* verificare la correttezza dell'ultima operazione col comando `git status`, dovrebbe fornire un messaggio simile:

        On branch master
        Your branch is up to date with 'origin/master'.

        nothing to commit, working tree clean

8. chiudere il terminale di Windows
9. avviare **TwinCAT3**
10. dal menu `File -> Apri... -> Progetto/Soluzione`, selezionare il progetto appena clonato ed aprirlo. 
Nel riquadro in basso a destra della finestra di TwinCAT3 XAE verrà indicato il nome del repository locale del progetto e il nome del branch attivo.
11. Nella finestra **Esplora soluzioni** rinominare la **soluzione** e il **progetto** (sulle prime due righe dell'albero della soluzione fare clic destro e `Rinomina`)
12. procedere con le modifiche del codice come richiesto dal nuovo progetto ed utilizzare i comandi della sezione **Team Explorer** di TwinCAT3 XAE per il commit e la sincronizzazione col repository remoto in GitHub.
