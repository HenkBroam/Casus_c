# README

Dit script vergelijkt verschillende populatiegroeimodellen door gebruik te maken van AIC (Akaike Informatiecriterium) en BIC (Bayesiaans Informatiecriterium), maar ook andere evaluatiemetrics zoals RMSE (Root Mean Squared Error) en de residuen. Het doel is om te evalueren hoe goed verschillende modellen de gegeven data voor tumorgroei over de tijd beschrijven. En dan het beste model te kiezen aan de hand van welke model het best scoort op de gegeven data. <Br>

### Modellen 
Geïmplementeerde Modellen:
Logistisch Groeimodel <br>
Gompertz Groeimodel <Br>
Von Bertalanffy Groeimodel <br>
Mendelsohn Groeimodel <Br>
Montroll Groeimodel <Br>
Allee Groeimodel <br>

### Gebruikte formules en methodes 
AIC (Akaike Informatiecriterium): Een maat voor de kwaliteit van het model in verhouding tot de data.<Br>
BIC (Bayesiaans Informatiecriterium): Vergelijkbaar met AIC, maar met een grotere straf voor modellen met meer parameters. <Br>    
RMSE (Root Mean Squared Error): Een maat voor hoe goed de modelvoorspellingen overeenkomen met de werkelijke data.<br>
Residuen: Het verschil tussen de voorspelde en werkelijke waarden, gebruikt om de nauwkeurigheid van het model te beoordelen.<br>
Visualisatie: Het script maakt een grafiek van de modelvoorspellingen samen met de werkelijke datapunten voor vergelijking.<br>

Numpy voor numpy dingen <br>
Matplotlib voor grafieken <br>
scipy voor Solve_IVP voor de tussenstappen van de datapunten berekenen <br>



### Gompertz en runge-kutta 
Het gompertz model is een sigmoide functie die veel wordt gebruikt voor biologische groei simulatie model. <br>
Dit is ook de reden dat dit model het beste uit de test kwam in dit onderzoekje. <br>
Formule: <br>
dV/dt = a * V * ln(b/V) <br>
V = volume <br> 
t = tijd <Br>
a = groeisnelheid <br>
b = aantal parameters (2) <br>

De Runge-Kutta methode is een numerieke techniek voor het oplossen van gewone differentiaalvergelijkingen (ODE's). Deze methode biedt een accurate benadering van de oplossing door herhaaldelijk kleine stappen te nemen. <Br>
In dit script wordt de 4e orde Runge-Kutta methode gebruikt om de Gompertz ODE op te lossen. <br>


### Gebruik 

Voor het gebruik van het script kan de gebruiker zelf data toevoegen om vervolgens het beste model te vinden. <br>
Wel moet de gebruiken de packages die boven staan geinstalleerd hebben <br>
Ook is kennis van de modellen handig in het kiezen van een model <br>
