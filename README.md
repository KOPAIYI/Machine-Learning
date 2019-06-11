# Machine-Learning

目標：人工智慧 <br>
手段：機器學習，讓機器具有學習的能力，可以讓機器跟人一樣有智慧。（深度學習 deep learning即為其中一個方法) <br>
--------------------------------------------------------------------------------------------
機器的本能：hand-crafted rule 人類設定好的天生本能<br>
weakness of hand-crafted rule<br>
  1.永遠無法超越創造者（因為都是靠創作者的想像力，一旦問題超過創作者的思考，即會出問題。）<br>
  2.需要很多的人力 <br>
  
What is Machine Learning? <br>
最簡單的說法就是寫一段程式讓他去學習  <br>
比較務實的說法就是：根據提供的資料，尋找一個我們需要的function（Machine Learning ~ Looking for a function from data)<br>

找出function的framework：<br>
  1.先準備一個function set（有無數的function），統稱funciton set為model <br>
  2.有一些訓練資料（training data），ex：function input:猴子的圖，output:猴子 <br>
  3.藉由上述的訓練資料，判斷model中的function是好還是不好的（透過Loss function：L）<br>
  
所以整個Machine Learning的framework：<br>
  1.訂出一個funciton set <br>
  2.讓machine衡量一個function好還是不好 <br>
  3.讓machine有一個好的演算法，可以挑出最好的function <br>
  
Supervised Learning包含了以下方法：<br>
  1.Regression -> the output of the target function f is "scalar" <br>

  2.Classification <br>
    -> Binary Classification：the output of the target function f is "yes or no" <br>
    -> Multi-class Classification：the output of the target function f is "class1,class2,...,class n"（簡單的說就是幫你選擇選項）<br>
    #Classification包含了linear model和non-linear model（Deep learning,SVM,Classifiaction tree,...）<br>
  3.Structured Learning-Beyond Classfication：<br>
    output為一個有結構性（複雜）的東西 <br>
    
Supervised Learning需要大量的training data，training data告訴我們input與ouput之間有什麼關係，而function output通常稱為label <br>

需要找到這些label通常需要很多人的努力，那如何去減少這些label所需求的effort，透過以下的方法：<br>
Semi-supervised learning：有少量的具有label的data，同時也有大量的unlabel的data，那在semi-supervised learning的技術裡面，這些unlabeled data對學習是有幫助的 <br>
Transfer learning：一樣具有少量的labeled data，同時有大量的unlabeled data，但與考慮的問題的label是沒什麼關係的，簡單來說就是不太相干，透過這些unlabeled data對學習有幫助 <br>
Unsupervised learning：給機器一堆unlabeled data，讓Machine舉一反三學會，輸出我們考慮的label <br>
Reinforcement learning：不告訴Machine正確答案是什麼，Machine所有的只是它做得好還是不好，而他也不知道哪裡做得好不好，他要回去看自己哪裡做錯了<br>

Supervised Learning v.s Reinforcement Learning：<br>
Supervised Learning就像是learning from teacher 就像是Machine旁邊有個老師教你，會告訴你正確答案，<br>
Reinforcement Learning是learning from critics，因為他不會知道正確答案，只會去記錄每次的評論，就比較像是我們人類真實的學習情境，所以現在比較受重視 <br>
比如 AlphaGO 就是supervised learning＋reinforcement learning，reinforcement learning需要一個對手，通常Machine的對手就是另一個Machine <br>
