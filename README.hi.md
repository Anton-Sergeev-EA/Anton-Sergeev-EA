[English](README.md) · [Русский](README.ru.md) · [中文](README.zh.md) · **हिन्दी** · [Español](README.es.md) · [العربية](README.ar.md) · [Français](README.fr.md) · [Português](README.pt.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [Italiano](README.it.md) · [Ελληνικά](README.el.md) · [Čeština](README.cs.md)

# अंतोन सर्गेयेव
### ML/DL और C++/Python इंजीनियर · औद्योगिक AI · विद्युत प्रणालियाँ और स्वचालन

**मैं मशीन लर्निंग, आधुनिक C++ और औद्योगिक इंजीनियरिंग के संगम पर सिस्टम विकसित करता हूँ।** मेरे काम में ML/DL मॉडल, नेटिव गणना, टेलीमेट्री पाइपलाइन और खोज प्रणालियाँ शामिल हैं—सिग्नल के अर्थ से लेकर उसे संसाधित करने वाले सॉफ्टवेयर के व्यवहार तक।

मेरा ध्यान कठिन इंजीनियरिंग समस्याओं पर है: शोरयुक्त डेटा, विफलता से पुनर्प्राप्ति, समवर्ती निष्पादन, मॉडल मूल्यांकन और मापने योग्य प्रदर्शन समझौते।

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

मैं परिचालन आवश्यकताओं को परीक्षण योग्य सॉफ्टवेयर अनुबंधों में बदलता हूँ, मॉडल को डेटा और बेसलाइन के संदर्भ में परखता हूँ और प्रदर्शन के दावे से पहले मापता हूँ।  सिंथेटिक ML प्रयोग तथा प्रयोगशाला प्रोटोकॉल परीक्षण केवल अपना घोषित दायरा दिखाते हैं; वास्तविक स्थल की सटीकता, तैनाती या प्रमाणन नहीं। हर रिपॉजिटरी अपनी सीमाएँ बताती है।

**संपर्क:** [avsergeev1981@gmail.com](mailto:avsergeev1981@gmail.com) · [Apollonian](https://apollonian.ru/) · [सभी रिपॉजिटरी](https://github.com/Anton-Sergeev-EA?tab=repositories)।
