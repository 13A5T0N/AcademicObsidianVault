# Confusion matrix 
- Stel: er zijn 2 categorieën
- we noemen deze “positive” en “negative”
-  er zijn 4 mogelijkheden
	- positive voorspeld, echte waarde is positive (True Positive)
	- positive voorspeld, echte waarde is negative (False Positive)
	- negative voorspeld, echte waarde is positive (False Negative)
	- negative voorspeld, echte waarde is negative (True Negative)
![[Pasted image 20240611042316.png]]

## Accuracy 
- we zoeken 1 getal dat uitdrukt hoe goed de voorspelling is
- accuracy is het aantal juiste voorspellingen gedeeld door het totaal aantal voorspellingen
$$ accuracy= TP+TN /TP+TN+FP+FN$$
## Precision en recall

- deze moeten beiden hoog zijn
- precision = hoeveel procent van de voorspelde positive waren ook daadwerkelijk positive?
- recall = hoeveel procent van de werkelijk positive werden ook als positive voorspeld

$$ precision= TP /TP+FP $$
$$ recall= TP / TP+FN $$
## F-measure

### Probleem
- precision en recall zijn 2 getallen
- ze moeten allebei zo hoog mogelijk zijn
- we willen maar 1 getal dat kan uitdrukken of ze beiden hoog zijn of niet
$$ Fβ= (β 2 +1)⋅P⋅R /β 2 ⋅P+R$$
- als β=1 dan spelen beiden evenveel mee
- als β>1 dan wordt er meer belang gehecht aan recall
- als β<1 dan wordt er meer belang gehecht aan precision


F1 wordt veel gebruikt:
$$ F 1 = 2 ⋅ P ⋅ R / P + R$$
# Andere maten
- False Positive Rate $$ (FPR) = FP / (TP + FN) $$
- True Positive Rate $$ (TPR) = TP / (TP + FN ) $$
	- dit is een andere benaming voor “recall”
- sensitivity $$ TP / (TP + FN) $$
	- dit is een andere benaming voor “recall”
- specificity $$ TN / (TN + FP) $$

# Orange
![[Pasted image 20240611043001.png]]


