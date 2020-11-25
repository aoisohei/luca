<h1 align='center'>Luca <br><br>  Распазнование человеческих эмоций<br> </h1> 
 
![](https://img.shields.io/badge/project-r1__elements-blue)

![](https://img.shields.io/badge/Windows-10-green) ![](https://img.shields.io/badge/Anaconda-3-green) ![](https://img.shields.io/badge/CUDA-10.1.-orange) ![](https://img.shields.io/badge/cuDNN-7.6.5-orange) ![](https://img.shields.io/badge/Python-3.8-blue) ![](https://img.shields.io/badge/TensorFlow-2.3.0-yellow) ![](https://img.shields.io/badge/TensorFlow-2.2.0-yellow) ![](https://img.shields.io/badge/Api-Custom%20Object%20Detection-blueviolet) ![](https://img.shields.io/badge/Year%20of%20creation-2020-blueviolet)

Projet comporte :
Partie 0.  **_Idée_**<br>
Partie 1.  **_DataSet_**<br>
Partie 2.  **_Model_**<br>
Partie 3.  **_Result_**<br>

Versions :  ![](https://img.shields.io/badge/Langue-Russian-blue) 
![](https://img.shields.io/badge/Langue-Fran%C3%A7ais-red) 
![](https://img.shields.io/badge/Langue-English-green)










<h3 align='center'>Partie 0.</h3>
<h1 align='center'>Idée</h1>
![](https://img.shields.io/badge/Langue-Russian-blue)

Все, кто знает игру Детроит, могли заметить, как в игре показывают в правом верхнем отношения между персонажами, напимер Отношение Хэнка к конору или отношени Иерихна к Маркусу. Это наталкнуло меня на мысль, что в любом роботе должна была внедрена программа, которая отвечаеи за понимание этих самых отношений, распазнавала бы эти самые отношения между людьми и распазнавала отношение человека к роботу, в котором внедреннв эта программа.<br>

Беззсомнено, именна это прогрмма делала б робота более человеченее, так как подразумевало, что робот способен сам анализировать эмоциональное состояние других людей и тех людей с которыми он общается и понимать, что они чувствуют в этот момент. Я считаю это полезная черта, и именно эту идею, я с командой Коммандой X̂ собираюсь реализовать в этом приложени: по сути наш "вооброжаем робот" по-имени Лука, которого еще нет, будет обучен распозновать эмоции по картинкам, это значит, что Лука, в будущей, при виде той или ситуации. Будет оценивать людей с превово взгляда и делать тот или иной вывод. От сюда вытекает большая проблема и недостаток моего приложения. Не все взаимоотношения, эмоции и уровни отшношений можно оценить по одним только картинком, например такое как "Доверий", которое всем извесно заваёвываеться годами (так что Конору ещё повезло с нопарником)! Или уровень отношений "Лидер" Маркуса, это тоже не та вещь, котоую можно распазнать с первово взгляда в человеке. Обычно такие вещи распазнаются по-поведению и общению. И это то чего на сей момент не может делать Лука.

Что же наша программа будем делать, это :

##### 1. Анализирываеть эмоциональное состояние человека, стоящего перед ним, или простым языком`

1. Радость,
2. Злость,
3. Отвращение,
4. Удивление,
5. Страх,
6. Грусть,
7. Жалость.

##### 2. Определять отношения человека к себе или отношение между людьми, которых он видит или коротко

1. Недоверие,
2. Любовь,
3. Дружба,
4. Близкие люди,
5. Деловые отношения - работают вместе,
6. Симпатия,
7. Подчинение\Прислуживвание

##### 3. А так же, конечно приложение будет распазновать уровни отношения человека, как этот делалось в Детроите, а потому я собрала все омоции, которые фигурировали в этой игре, а именно:

1. Лидер \ Leader(Admired)
2. Уважение \ Respected
3. Любовь \ Lover
4. Напарник \ Companion
5. Семья \ Family
6. Друзья \ Friend
7. Теплые отношения \ Warm
8. Нейтральное отношение \ Neutral
9. Неопределенный отношения \ Resentful
10. Близкие отношения \ Close
11. Напряженные отшношения \ Tense
12. Не заслуживает доверия \ Distrusted

***
 
<h3 align='center'>Partie 1.</h3>
<h1 align='center'>DataSet</h1>


<p align='center'>Tache principale:</p>
**<h3 align='center'>Trouve boeucoup des donées</h3>**
***
Là ce sont mes notes sur les persoones qui ont déjà appris cette question :
- Need explore image of emotion : https://www.kaggle.com/gauravsharma99/facial-emotion-recognition?select=fer2013
- Audio Imachine https://www.kaggle.com/ejlok1/audio-emotion-part-1-explore-data
- Ici il y beaucoup d'audios :
  - https://www.kaggle.com/ejlok1/surrey-audiovisual-expressed-emotion-savee 
  - https://www.kaggle.com/ejlok1/cremad
  - https://www.kaggle.com/uwrfkaggler/ravdess-emotional-speech-audio 
  - https://www.kaggle.com/ejlok1/toronto-emotional-speech-set-tess
- https://www.kaggle.com/shivamburnwal/speech-emotion-recognition
- Un model - https://www.kaggle.com/ritzing/speech-emotion-recognition-with-cnn
- Training of model - https://www.kaggle.com/ejlok1/audio-emotion-part-3-baseline-model
- Les sons - https://www.kaggle.com/iwilldoit/emotions-sensor-data-set
- Les mots - https://www.kaggle.com/praveengovi/emotions-dataset-for-nlp 
- Les etats - https://www.kaggle.com/ishivinal/tweet-emotions-analysis-using-lstm-glove-roberta/comments
- https://www.kaggle.com/milan400/human-emotion-detection-by-using-cnn/comments
- https://www.kaggle.com/nikitaivanov/predicting-emotions
- https://www.kaggle.com/ishivinal/tweet-emotions-analysis-using-lstm-glove-roberta
- https://www.kaggle.com/hexmag/emotion-sensor
- https://www.kaggle.com/dataturks/face-dataset-with-age-emotion-ethnicity
- https://www.kaggle.com/sankha1998/emotion
- https://www.kaggle.com/ishivinal/tweet-emotions-analysis-using-lstm-glove-roberta/comments
- https://www.kaggle.com/milan400/human-emotion-detection-by-using-cnn
- https://www.kaggle.com/sanikamal/predict-emotional-sentiment

P.S.:
Свои вопросы Луке:
- Какая втоя любимоя музыка ? (что любишь слушать)
- Как запихнуть слона в холодильник
 
 
<h3 align='center'>Partie 2.</h3>
<h1 align='center'>Model</h1>


### Intruduction

Значит, делаем приложение для распознавания неважно какого набора данных на Tensorflow 2, план :

* Setting up Anaconda, CUDA, and cuDNN
* Installing TensorFlow
* Preparing our Workspace and Virtual Environment Directory Structure
* Preparing the Dataset
* Configuring the Training Pipeline
* Training the Model
* Exporting the inference graph
* Testing and using your newly trained object detection classifier

Сразу скажу, что я сама училась на основе этого ролика :

* [https://www.youtube.com/watch?v=oqd54apcgGE&t=1291s](https://www.youtube.com/watch?v=oqd54apcgGE&t=1291s) ,
* [https://github.com/armaanpriyadarshan/Training-a-Custom-TensorFlow-2.x-Object-Detector](https://github.com/armaanpriyadarshan/Training-a-Custom-TensorFlow-2.x-Object-Detector)<br>
Все файлы, которые я скачивала или и сохраняла отдельно на гугл диске.

***

### Setting up Anaconda, CUDA, and cuDNN

Setting up Anaconda, CUDA, and cuDNN<br>

Если у вас<br>

![alt text](https://github.com/%5Busername%5D/%5Breponame%5D/blob/%5Bbranch%5D/image.jpg?raw=true)

### Installing TensorFlow

Setting up Anaconda, CUDA, and cuDNN

### Preparing our Workspace and Virtual Environment Directory Structure

Setting up Anaconda, CUDA, and cuDNN

### Preparing the Dataset

Setting up Anaconda, CUDA, and cuDNN

### Configuring the Training Pipeline

Setting up Anaconda, CUDA, and cuDNN

### Training the Model

Setting up Anaconda, CUDA, and cuDNN

### Exporting the inference graph

Setting up Anaconda, CUDA, and cuDNN

### Testing and using your newly trained object detection classifier

Setting up Anaconda, CUDA, and cuDNN


<h3 align='center'>Partie 3.</h3>
<h1 align='center'>Result</h1> 


