[English](README.md) · [Русский](README.ru.md) · [中文](README.zh.md) · [हिन्दी](README.hi.md) · [Español](README.es.md) · [العربية](README.ar.md) · [Français](README.fr.md) · [Português](README.pt.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [Italiano](README.it.md) · **Ελληνικά** · [Čeština](README.cs.md)

# Άντον Σεργκέεφ
### Μηχανικός ML/DL και C++/Python · Βιομηχανική AI · Ενέργεια και αυτοματισμός

**Αναπτύσσω συστήματα στη διασταύρωση της μηχανικής μάθησης, της σύγχρονης C++ και της βιομηχανικής μηχανικής.** Τα έργα μου συνδυάζουν μοντέλα ML/DL, εγγενείς υπολογισμούς, τηλεμετρία και συστήματα αναζήτησης—από τη σημασία ενός σήματος μέχρι τη συμπεριφορά του λογισμικού που το επεξεργάζεται.

Εστιάζω στις δύσκολες τεχνικές προκλήσεις: θορυβώδη δεδομένα, ανάκαμψη από αστοχίες, ταυτόχρονη εκτέλεση, αξιολόγηση μοντέλων και μετρήσιμους συμβιβασμούς απόδοσης.

## Επιλεγμένα τεχνικά έργα

### [ARGUS-NEURO](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO) — μηχανική μάθηση για διάγνωση εξοπλισμού
Χαρακτηριστικά σημάτων σε C++20 μέσω pybind11, κλασική ανίχνευση ανωμαλιών, μοντέλα PyTorch LSTM/GRU και συμπερασμός ONNX. Τεκμηριώνονται οι διαχωρισμοί δεδομένων, τα μοντέλα αναφοράς, η προέλευση δεδομένων και η αποχή από ανεπαρκώς τεκμηριωμένες εκτιμήσεις.

**Για έλεγχο:** [σύμβαση αξιοπιστίας](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/main/docs/RELIABILITY.md) · [αρχεία πειραμάτων](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/tree/main/experiments) · [CI](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/actions).

### [Ironpulse](https://github.com/Anton-Sergeev-EA/Ironpulse) — ανθεκτική βιομηχανική τηλεμετρία σε C++20
Ασύγχρονη συλλογή Modbus TCP, χρονικά όρια και επανασύνδεση, αποθήκευση WAL, στατιστική ανίχνευση ανωμαλιών και διεπαφές REST/WebSocket. Έμφαση στη συμπεριφορά κατά τις αστοχίες επικοινωνίας και αποθήκευσης.

**Για έλεγχο:** [δοκιμές](https://github.com/Anton-Sergeev-EA/Ironpulse/tree/main/tests) · [μεταγλώττιση, sanitizers και ολοκλήρωση](https://github.com/Anton-Sergeev-EA/Ironpulse/actions).

### [Cognivore](https://github.com/Anton-Sergeev-EA/Cognivore) — τοπική αναζήτηση εγγράφων και RAG
Ακριβή/προσεγγιστικά διανυσματικά ευρετήρια σε C++ με σύνδεση Python, embeddings, BM25 και API. Οι δοκιμές ευρετηρίων και οι μετρήσεις συγκεκριμένων φορτίων επιτρέπουν τον έλεγχο της αναζήτησης και των συμβιβασμών απόδοσης.

**Για έλεγχο:** [εγγενής υλοποίηση](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/native) · [μετρήσεις απόδοσης](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/benchmarks) · [CI](https://github.com/Anton-Sergeev-EA/Cognivore/actions).

### Πρόσθετα συστήματα

- **[GridGuard](https://github.com/Anton-Sergeev-EA/GridGuard):** Εργαστήριο IEC 61850 MMS/URCB, ποιότητα τηλεμετρίας, WAL με προστασία CRC και επανεγγραφή στη βάση δεδομένων.
- **[SCADA_Generator](https://github.com/Anton-Sergeev-EA/SCADA_Generator):** HMI από παραμετροποίηση, προσαρμογείς βιομηχανικών πρωτοκόλλων, κύκλος ζωής συναγερμών και ανάλυση C++/Python.
- **[adaptive_capacity_allocator](https://github.com/Anton-Sergeev-EA/adaptive_capacity_allocator):** Πολιτικές αύξησης χωρητικότητας περιεκτών C++17/20 με αναπαραγώγιμες μετρήσεις μνήμης και χρόνου.

## Τεχνικά εργαλεία

| Τομέας | Τεχνολογίες και μέθοδοι |
|---|---|
| Μηχανική και βαθιά μάθηση | PyTorch, scikit-learn, LightGBM/XGBoost, LSTM/GRU, ανωμαλίες, χρονοσειρές, PCA, ONNX |
| Λογισμικό και δεδομένα | C++17/20, Python, CMake, pybind11, FastAPI, REST/WebSocket, PostgreSQL, SQLite |
| Αναζήτηση και παράδοση | RAG, embeddings, BM25, διανυσματική αναζήτηση, Linux, Docker, GitHub Actions, pytest, CTest, Ruff, sanitizers |

## Τεχνική προσέγγιση

Μετατρέπω λειτουργικές απαιτήσεις σε ελέγξιμες συμβάσεις λογισμικού, αξιολογώ μοντέλα ως προς τα δεδομένα και τα μοντέλα αναφοράς και μετρώ πριν διατυπώσω ισχυρισμούς απόδοσης. Τα πειράματα ML με συνθετικά δεδομένα και οι εργαστηριακές δοκιμές πρωτοκόλλων τεκμηριώνουν το δηλωμένο εύρος τους, όχι ακρίβεια πεδίου, εγκατάσταση ή πιστοποίηση. Κάθε αποθετήριο περιγράφει τους περιορισμούς του.

**Επικοινωνία:** [kavery@mail.ru](mailto:kavery@mail.ru) · [Apollonian](https://apollonian.ru/) · [όλα τα αποθετήρια](https://github.com/Anton-Sergeev-EA/?tab=repositories).
