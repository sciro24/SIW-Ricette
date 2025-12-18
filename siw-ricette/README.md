# <img src="src/main/resources/static/images/logo-siw.png" alt="SIW Ricette Logo" width="40" height="40" style="vertical-align: bottom;" /> SIW Ricette

Benvenuto in **SIW Ricette**, una piattaforma web dedicata alla condivisione e alla scoperta di ricette culinarie. Questo progetto è stato sviluppato come applicazione web completa, gestendo l'intero ciclo di vita del dato, dalla persistenza alla presentazione all'utente finale.

## 🎯 Obiettivo del Progetto

L'obiettivo principale è fornire un sistema centralizzato dove:
- Gli **Chef (Amministratori)** possono gestire il catalogo, inserendo nuove ricette e ingredienti.
- I **Cuochi (Utenti Registrati)** possono esplorare il catalogo e lasciare recensioni sui piatti.
- I **Visitatori** possono consultare le ricette e cercare ispirazione culinaria.

## 🛠️ Tecnologie Utilizzate

Il progetto è costruito su uno stack tecnologico moderno basato sull'ecosistema Java:

### Backend
*   **Java**: Linguaggio di programmazione principale.
*   **Spring Boot**: Framework per lo sviluppo rapido di applicazioni.
*   **Spring Data JPA**: Per la gestione della persistenza dei dati e l'astrazione del database.
*   **Spring Security**: Per la gestione dell'autenticazione e delle autorizzazioni (Utenti vs Admin).

### Frontend
*   **Thymeleaf**: Template engine Java per generare viste HTML dinamiche lato server.
*   **HTML5 & CSS3**: Per la struttura e lo stile delle pagine (fogli di stile personalizzati in `static/css`).
*   **Bootstrap** (se presente) o CSS Custom per il layout responsive.

### Build & Tools
*   **Maven**: Per la gestione delle dipendenze e il build del progetto.

## ✨ Funzionalità Principali

### 👤 Area Pubblica & Utente
*   **Catalogo Ricette**: Visualizzazione di tutte le ricette disponibili con dettagli e foto.
*   **Ricerca**: Funzionalità per cercare ricette specifiche.
*   **Recensioni**: Gli utenti autenticati possono lasciare recensioni e valutazioni sulle ricette.
*   **Registrazione & Login**: Sistema sicuro per la creazione di account personali.

### 🛡️ Area Amministratore
*   **Gestione Ricette**: Creazione, modifica e cancellazione delle ricette.
*   **Gestione Ingredienti**: Aggiunta e gestione degli ingredienti disponibili nel sistema.
*   **Associazione**: Strumenti per associare ingredienti specifici alle ricette.

## 🚀 Come avviare il progetto

1.  Assicurati di avere **Java (JDK 17 o superiore)** installato.
2.  Clona il repository o scarica il progetto.
3.  Apri un terminale nella cartella radice del progetto.
4.  Esegui il comando Maven per avviare l'applicazione:

    ```bash
    ./mvnw spring-boot:run
    ```

5.  Una volta avviato, apri il browser e vai su:
    `http://localhost:8080`

## 📂 Struttura del Progetto

```text
src/main/java
├── authentication  # Configurazione della sicurezza
├── controller      # Gestione delle richieste HTTP
├── model           # Entità del dominio (Ricetta, Ingrediente, ecc.)
├── repository      # Interfacce per l'accesso ai dati
└── service         # Logica di business
```

---
*Progetto sviluppato per il corso di Sistemi Informativi su Web - Università Roma Tre.*
