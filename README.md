# Classe_Albero: Creazione di una Classe Albero Binario con Vettori

#### 1. Implementare una classe che rappresenti una struttura dati ad **Albero Binario**:

Rappresentato utilizzando un array con la relazione tra genitori e figli:
     - Il **figlio sinistro** di un nodo all'indice \(i\) si trova all'indice \(2i+1\).
     - Il **figlio destro** di un nodo all'indice \(i\) si trova all'indice \(2i+2\).

  Implementare le seguenti operazioni di base:
   - Inserimento della radice.
   - Verifica se l'albero è vuoto.
   - Leggere radice.
   - Verifica se un nodo è foglia.
   - Accesso al figlio sinistro e destro, dato l'indice di un nodo.
   - Aggiunta di nuovi figli, se non presenti.
   - Rimozione di un nodo dato il suo indice e solo se é foglia.
   - Stampa del tipo: "Pos 0, Valore: ..., Figliodestro: ..., Figliosinistro: ..."

---

Dettagli dell'Esercizio:

**Classe per l'Albero Binario**:
   - Utilizza un array lineare per rappresentare l'albero:
     - L'indice \(0\) rappresenta la radice.
     - La relazione tra i nodi segue la regola \(2i+1\) (figlio sinistro) e \(2i+2\) (figlio destro)
---

Anteprima della Classe:

**Albero Binario:**
```cpp
template <typename T>
class AlberoBinario {
private:
    T nodi[100];
public:
    AlberoBinario();
    bool alberoVuoto() const;
    void insRadice(const T& valore);
    T radice() const;
    bool isFoglia(int indice) const;
    int figlioSinistro(int indice) const;
    int figlioDestro(int indice) const;
    void insFiglioSinistro(int indice, const T& valore);
    void insFiglioDestro(int indice, const T& valore);
    void rimuovi(int indice);
    void stampa() const;
};
```

---

#### 2. Programma Principale (main): 
Testare gli operatori creati su un albero a piacere (caricare nel repository GitHub il disegno (fatelo come preferite) dell'albero utilizzato nel main. Tutti gli alberi devono essere diversi).
   - Creazione di un albero con radice.
   - Inserimento di nodi figli.
   - Accesso ai figli (per N-ario) o ai figli sinistro e destro (per Binario).
   - Rimozione di un nodo.
   - Stampa della struttura dell'albero.
   - Caricare nel repository GitHub il disegno (fatelo come preferite) dell álbero utilizzato nel main.

---
