# Rolbeheerstelsel vir sweeftuig

Stelsel wat die vlerke gelyk hou in rol.  Rolhoek word met 'n 3-assige versnellingsmeter gemeet en dit word dan beheer terug na 'n 0 grade rolhoek deur die aanwending van rolroere wat met servos beheer word.





![AirfoilGlideAngle](Prente\AirfoilGlideAngle.png)
$$
T = C_r \delta
$$

$$
\ddot{\theta} = \frac{T}{I_{xx}}
$$

Waar $\theta$ die heihoek is.

Die volgende diagram beskryf die beheerstelsel:

![ControlLoopRoll](Prente\ControlLoopRoll.png)

Daar is filters nodig om die metings te filter met die volgende oordragsfunksie.  Dit is nog nie in die diagram nie.

$H(s)=\frac{1}{1+sA}$

Die beheerstelsel is digitaal dus word daar van die z-transform gebruik om die digitale beheerstelsel te analiseer:

$h(t) \rightarrow H(s) \rightarrow H(z)$

Die digitale beheer het 'n ekstra filter effek wat dit inbring.  Die volgende diagram is nog nie reg/volledig nie, maar dit is soos die diagram van die s- na die z-transform gaan:

![FilterEffek](Prente\FilterEffek.png)

Where $\theta$ is the pitch angle.




# Te doen

Maak 'n draad op waarmee die servo en die versnellingsmeter gelyk in die 5V krag kan inprop.  Onthou 2 servos.
Maak seker Arduino kan genoeg stroom gee vir die servos en versnellingsmeter
Sit tweede servo by in program
Teken stroombaan in Fritzing (dus vertaal Fritzing en teken stroombaan en dan sit dit in hierdie dokument)

Die servo uitset het baie geraas.  Vind uit waar dit vandaan kom.  Miskien moet daar 'n filter kom
