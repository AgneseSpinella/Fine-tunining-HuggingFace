# Fine-tunining-HuggingFace

L’obiettivo di questo progetto è eseguire il fine-tuning di due modelli pre-allenati sfruttando un 
dataset di Hugging Face. Il dataset scelto è composto da due features:  
• “text”: è di tipo stringa. Un record è composto da una domanda e da un’affermazione 
• “label”: è di tipo integer. Assume il valore 0 se l’affermazione non fornisce informazioni 
pertinenti e sufficienti alla domanda posta, mentre assume il valore 1 in caso contrario. 

Esempio: 
Sentence: The cat lived with Jeremy, along with his orange and black cat.  
Question: Where did Jeremy find the cat?"   0 

"Sentence: Two of her friends were going to the nearby beach to do some swimming and 
enjoy the sun.  
Question: Where did Jenny and her friends lay down on the towels to enjoy the sun?"   1 

Lo scopo del fine-tuning da effettuare è dunque quello di fare in modo che il modello allenato riesca 
a determinare se l'asserzione fornisce informazioni inerenti alla domanda a cui è collegata.  
Lo sviluppo di questo task potrebbe rivelarsi utile nell’ambito dell’NLP e trovare applicazione in 
diversi ambiti, ad esempio nel campo dello studio delle risposte automatiche o della verifica della 
coerenza domanda/risposta. 
Il dataset è consultabile al link: https://huggingface.co/datasets/mattymchen/natural-instruction-
050, mentre il codice da cui sono stati estratti gli script per questa relazione è consultabile al link: 
https://colab.research.google.com/drive/1jK_RIA2XvyLFogFubG_ruNWHOajeLO6_?usp=sharing  
