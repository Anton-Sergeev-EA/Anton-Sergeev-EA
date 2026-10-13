[English](README.md) · [Русский](README.ru.md) · [中文](README.zh.md) · **हिन्दी** · [Español](README.es.md) · [العربية](README.ar.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [Italiano](README.it.md)

# अंतोन सर्गेयेव
### ML/DL और C++/Python इंजीनियर · औद्योगिक AI · विद्युत प्रणालियाँ और स्वचालन

**मैं औद्योगिक क्षेत्र के ज्ञान को सॉफ्टवेयर इंजीनियरिंग और मशीन लर्निंग से जोड़ता हूँ।** मेरे अनुभव में विद्युत उपकरणों का निदान, प्रक्रिया स्वचालन और तकनीकी परियोजनाओं का नेतृत्व शामिल है। आज मैं निगरानी, पूर्वानुमान और इंजीनियरिंग निर्णयों में सहायता के लिए ML/DL मॉडल, नेटिव कंप्यूटिंग मॉड्यूल और डेटा सेवाएँ विकसित करता हूँ।

मेरी ताकत पूरी समस्या को समझना है: माप का अर्थ, उपकरण की विफलता के तरीके, मॉडल तक डेटा का प्रवाह और कनेक्शन या घटक विफल होने पर सॉफ्टवेयर का व्यवहार।

## पेशेवर अनुभव

- **2001–2023 · इंजीनियरिंग और नेतृत्व:** **0.4–750 kV** विद्युत उपकरणों का निदान, जिसमें आंशिक डिस्चार्ज और डाइइलेक्ट्रिक हानि के माप शामिल हैं; बड़ी औद्योगिक परियोजनाओं में स्वचालन कार्यों का नेतृत्व।
- **औद्योगिक परियोजनाएँ:** टोबोल्स्क में SIBUR के पॉलीप्रोपिलीन संयंत्र और Gazprom की **120 MW विद्युत संयंत्र परियोजना** का स्वचालन; Leningrad NPP-2 और Lavna बंदरगाह सहित परियोजनाओं में विद्युत, नियंत्रण और संचार कार्य।
- **सितंबर 2024 से · Apollonian:** ML इंजीनियरिंग और परियोजना नेतृत्व; कंपन, दबाव और तापमान टेलीमेट्री के लिए LSTM और ग्रेडिएंट बूस्टिंग मॉडल; डेटा बफरिंग, S3 अभिलेख और REST/WebSocket एकीकरण।
- **शिक्षा:** Peter the Great St. Petersburg Polytechnic University से विद्युत ऊर्जा इंजीनियरिंग में मास्टर डिग्री, **2021**। ML/DL, कंप्यूटर विज़न, RAG, C++, Python और DevOps में अतिरिक्त प्रशिक्षण।

औद्योगिक अनुभव मेरी सॉफ्टवेयर आवश्यकताओं की समझ को आकार देता है; नीचे दिए गए सार्वजनिक रिपॉजिटरी कार्यान्वयन और मूल्यांकन के उदाहरण प्रस्तुत करते हैं।

## चुनिंदा इंजीनियरिंग परियोजनाएँ

### [ARGUS-NEURO](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO) — उपकरण निदान के लिए मशीन लर्निंग
pybind11 के माध्यम से C++20 सिग्नल फीचर, पारंपरिक विसंगति पहचान, PyTorch LSTM/GRU और ONNX इन्फरेंस। डेटा विभाजन, बेसलाइन, डेटा का स्रोत और पर्याप्त प्रमाण न होने पर अनुमान देने से इनकार करने की व्यवस्था दस्तावेज़ों में स्पष्ट हैं।

**देखें:** [विश्वसनीयता अनुबंध](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/main/docs/RELIABILITY.md) · [प्रयोग के परिणाम और विन्यास](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/tree/main/experiments) · [CI](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/actions)।

### [Ironpulse](https://github.com/Anton-Sergeev-EA/Ironpulse) — C++20 में विश्वसनीय औद्योगिक टेलीमेट्री
असिंक्रोनस Modbus TCP संग्रह, टाइमआउट और पुनः कनेक्शन, WAL स्टोरेज, सांख्यिकीय विसंगति पहचान तथा REST/WebSocket इंटरफेस। संचार या स्टोरेज विफल होने पर उपयोगी व्यवहार बनाए रखना इसका मुख्य लक्ष्य है।

**देखें:** [परीक्षण](https://github.com/Anton-Sergeev-EA/Ironpulse/tree/main/tests) · [बिल्ड, सैनिटाइज़र और एकीकरण CI](https://github.com/Anton-Sergeev-EA/Ironpulse/actions)।

### [Cognivore](https://github.com/Anton-Sergeev-EA/Cognivore) — स्थानीय दस्तावेज़ खोज और RAG
Python से जुड़े C++ सटीक/अनुमानित वेक्टर इंडेक्स, embeddings, BM25 और API। इंडेक्स परीक्षण तथा विशिष्ट वर्कलोड के बेंचमार्क खोज व्यवहार और प्रदर्शन के समझौतों को स्पष्ट करते हैं।

**देखें:** [नेटिव कार्यान्वयन](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/native) · [बेंचमार्क](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/benchmarks) · [CI](https://github.com/Anton-Sergeev-EA/Cognivore/actions)।

### अन्य सिस्टम परियोजनाएँ

- **[GridGuard](https://github.com/Anton-Sergeev-EA/GridGuard):** IEC 61850 MMS/URCB प्रयोगशाला, टेलीमेट्री गुणवत्ता, CRC-सुरक्षित WAL और डेटाबेस रीप्ले।
- **[SCADA Generator](https://github.com/Anton-Sergeev-EA/SCADA_Generator):** कॉन्फ़िगरेशन से HMI, औद्योगिक प्रोटोकॉल एडाप्टर, अलार्म जीवनचक्र और C++/Python विश्लेषण।
- **[Adaptive capacity allocator](https://github.com/Anton-Sergeev-EA/adaptive_capacity_allocator):** C++17/20 कंटेनर वृद्धि नीतियाँ और दोहराए जा सकने वाले मेमोरी/समय माप।

## तकनीकी उपकरण

| क्षेत्र | तकनीक और विधियाँ |
|---|---|
| मशीन लर्निंग और डीप लर्निंग | PyTorch, scikit-learn, LightGBM/XGBoost, LSTM/GRU, विसंगति पहचान, टाइम सीरीज़, PCA, ONNX |
| सॉफ्टवेयर और डेटा | C++17/20, Python, CMake, pybind11, FastAPI, REST/WebSocket, PostgreSQL, SQLite |
| खोज और डिलीवरी | RAG, embeddings, BM25, वेक्टर खोज, Linux, Docker, GitHub Actions, pytest, CTest, Ruff, सैनिटाइज़र |

## काम करने का तरीका

मैं परिचालन आवश्यकताओं को परीक्षण योग्य सॉफ्टवेयर अनुबंधों में बदलता हूँ, मॉडल को डेटा और बेसलाइन के संदर्भ में परखता हूँ और प्रदर्शन के दावे से पहले मापता हूँ। **औद्योगिक नौकरी का अनुभव और सार्वजनिक परियोजना का सत्यापन अलग हैं:** सिंथेटिक ML प्रयोग तथा प्रयोगशाला प्रोटोकॉल परीक्षण केवल अपना घोषित दायरा दिखाते हैं; वास्तविक स्थल की सटीकता, तैनाती या प्रमाणन नहीं। हर रिपॉजिटरी अपनी सीमाएँ बताती है।

## काम और सहयोग

**ML/DL इंजीनियरिंग, C++/Python विकास और औद्योगिक AI** में रुचि: निदान, पूर्वानुमान, खोज प्रणालियाँ, टेलीमेट्री और विश्वसनीय डेटा सेवाएँ। स्थानांतरण और अंतरराष्ट्रीय टीमों के साथ काम के लिए तैयार हूँ।

**संपर्क:** [kavery@mail.ru](mailto:kavery@mail.ru) · [Apollonian](https://apollonian.ru/) · [सभी रिपॉजिटरी](https://github.com/Anton-Sergeev-EA?tab=repositories)।
