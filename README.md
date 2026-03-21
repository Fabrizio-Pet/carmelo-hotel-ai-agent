# carmelo-hotel-ai-agent

# 🏨 Carmelo: Hotel's Reservation Agent
**L'intelligenza artificiale al servizio dell'ospitalità 4.0**

Carmelo è un agente AI avanzato progettato per rivoluzionare la gestione delle prenotazioni alberghiere. Nato dalla necessità di ottimizzare il lavoro dei receptionist, Carmelo gestisce in autonomia la comunicazione con i clienti, la verifica delle disponibilità e l'inserimento delle prenotazioni nel database, garantendo risposte rapide e precise 24/7.

---

## 🚀 Funzionalità Principali
* **Gestione Prenotazioni Automatica:** Dialoga con l'utente per raccogliere date, numero di ospiti e preferenze.
* **Integrazione Database:** Verifica in tempo reale la disponibilità delle camere e registra i dati su PostgreSQL.
* **Supporto Multicanale:** Progettato per essere integrato via Chatbot (Telegram/Web) e gestire notifiche istantanee.
* **Customer Satisfaction:** Riduce drasticamente i tempi di attesa e previene l'overbooking grazie alla sincronizzazione automatica.

---

## 🛠️ Tech Stack
Il cuore di Carmelo batte grazie a un'architettura moderna e scalabile:

* **Orchestrazione:** [n8n](https://n8n.io/) (Workflow automation)
* **Cervello AI:** OpenAI GPT-4 / LangChain (tramite nodi AI di n8n)
* **Database:** [PostgreSQL](https://www.postgresql.org/) (Gestione inventario camere e clienti)
* **Storage & Cloud:** Supabase / n8n.cloud
* **Comunicazione:** Telegram API / Webhook personali

---

## 🧠 Architettura del Sistema
Il sistema è diviso in tre moduli logici fondamentali:

1.  **Modulo di Comprensione:** L'AI analizza il linguaggio naturale dell'utente (NLP) per estrarre entità (check-in, check-out, tipo camera).
2.  **Modulo Logico:** n8n interroga il database PostgreSQL per confermare che i parametri richiesti siano disponibili.
3.  **Modulo di Scrittura:** Una volta confermato l'interesse del cliente, l'agente scrive la prenotazione nel DB e invia una conferma formale.


   ![Descrizione Immagine](./assets/n8n-workflow-full.png)

---

## 📈 Impatto e Obiettivi
* **Efficienza Operativa:** Riduzione del 70% del carico di lavoro manuale per le prenotazioni standard.
* **Scalabilità:** Possibilità di gestire centinaia di richieste simultanee senza errori umani.
* **Zero-Loss:** Nessuna richiesta viene persa, ogni lead viene gestito dal bot o passato all'operatore in caso di complessità.

---

## 👥 Il Team
Progetto realizzato con passione per il **Concorso "Premio Di Bartolo"** da:
* Fabrizio Petralia (Captain)- Backend & AI Integration
* Manuel Di Pino- Database creation
* Martina Lo Giudice- Frontend structure

---

