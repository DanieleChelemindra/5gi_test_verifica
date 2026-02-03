# 5gi_test_verifica

Perfetto 👍 ti faccio **appunti ordinati e chiari** su **Git Bash + Git**, seguendo esattamente quello che hai fatto. Ideali da studiare per verifica 👇

---

## 📁 Comandi base del terminale (Git Bash)

### `mkdir nome_cartella`

Crea una nuova cartella.

```bash
mkdir 5gi_test_verifica
```

---

### `ls`

Elenca file e cartelle della directory corrente.

```bash
ls
```

### `ls /`

Mostra il contenuto della **root** del sistema Git Bash.

---

### `cd nome_cartella`

Entra in una cartella.

```bash
cd 5gi_test_verifica/
```

### `cd`

Se usato male (senza parametri validi) **non cambia cartella**.
Per tornare indietro:

```bash
cd ..
```

---

### `touch nomefile`

Crea un file vuoto.

```bash
touch esempio1.txt
```

---

### `cat nomefile`

Mostra il contenuto di un file.

```bash
cat esempio1.txt
```

⚠️ `type` su Git Bash **non funziona come su Windows CMD**.

---

### `vim nomefile`

Apre il file con l’editor **vim** (editor testuale).

* `i` → scrivere
* `ESC` → uscire dalla modalità scrittura
* `:wq` → salva ed esce

---

## 🌐 Git – Repository

### `git clone URL`

Clona un repository remoto (GitHub) in locale.

```bash
git clone https://github.com/DanieleChelemindra/5gi_test_verifica.git
```

❌ Errore:

```bash
git clone
```

➡️ **Devi specificare l’URL del repository**

---

## 📄 Stato del progetto

### `git status`

Mostra:

* branch corrente
* file modificati
* file non tracciati

```bash
git status
```

---

### `git diff`

Mostra le **differenze** tra file modificati e ultimo commit.

```bash
git diff
```

---

## ➕ Aggiungere file all’area di staging

### `git add nomefile`

Aggiunge un file allo staging.

```bash
git add esempio1.txt
```

### `git add .`

Aggiunge **tutti** i file modificati.

```bash
git add .
```

⚠️ Warning `LF → CRLF`
Normale su Windows, **non è un errore**.

---

## 💾 Commit

### `git commit -m "messaggio"`

Salva definitivamente le modifiche.

```bash
git commit -m "primo commit"
```

❌ `git commit ?` → comando errato

❌ Commit senza messaggio → Git lo blocca

---

## 🏷️ Tag

### `git tag -a nome -m "messaggio"`

Crea un **tag annotato** (es. versione).

```bash
git tag -a v2.3ReleaseMinor -m "aggiornamento release"
```

### `git show nome_tag`

Mostra info del tag + commit associato.

```bash
git show v2.3ReleaseMinor
```

---

## 🌿 Branch

### `git branch`

Mostra tutti i branch.

```bash
git branch
```

### `git branch nome`

Crea un nuovo branch.

```bash
git branch Chelemindra
```

---

### `git checkout nome_branch`

Cambia branch.

```bash
git checkout Chelemindra
```

---

## 🔀 Merge

### `git merge nome_branch`

Unisce un branch nel branch corrente.

```bash
git merge Chelemindra
```

✔️ **Fast-forward**: merge automatico senza conflitti
❌ `Already up to date` → non c’è nulla da unire

---

## 🌍 Remote

### `git remote -v`

Mostra repository remoto collegato.

```bash
git remote -v
```

---

## 🧠 Cose importanti da ricordare (da verifica)

* `clone` = scaricare progetto da GitHub
* `add` = preparare i file
* `commit` = salvare uno snapshot
* `branch` = linea di sviluppo separata
* `merge` = unire branch
* `tag` = versione del progetto
* `status` e `diff` = **fondamentali**

