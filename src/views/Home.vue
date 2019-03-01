<template>
  <v-app>

  <div class="home">
    <h2>Personlighetsanalys av drivande behov</h2><br>
    <p>Poängsätt varje påstående med följande svar ”Nej”, ”Delvis” eller ”Ja”.<br>
    Det är viktigt att vara helt ärlig när du utvärderar hur väl påståendet stämmer in på dig enligt följande kriterier:<br>
    Ja – ”detta stämmer verkligen in på mig.”<br>
    Delvis – ”detta stämmer delvis in på vem jag är”<br>
    Nej – ”Detta stämmer sannolikt inte in på vem jag är”.<br>
    Om du är osäker på ditt svar är det bäst om du väljer alternativet ”Nej”<br>
</p>


    <!--<img alt="Vue logo" src="../assets/logo.png">-->
        <!-- v-model="valid" -->
        <v-form>
            <!--<label for="name">Name of food:  </label>-->
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>1. Jag imponerar på andra</h3>
                      <v-radio-group v-model="answer[0]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>2. Tillhörighet är viktigt för mig</h3>
                      <v-radio-group v-model="answer[1]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>3. Att ha en tryggt hem är viktigt för mig</h3>
                      <v-radio-group v-model="answer[2]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>4. Jag tar gärna risker</h3>
                      <v-radio-group v-model="answer[3]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>5. Jag är inte rädd för förändringar, stämmer det?</h3>
                      <v-radio-group v-model="answer[4]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>6. Så länge man fortsätter att försöka kan man inte misslyckas</h3>
                      <v-radio-group v-model="answer[5]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>7. Jag tycker det är viktigt att kunna bidra och ge tillbaka</h3>
                      <v-radio-group v-model="answer[6]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>8. Jag är bra på att ta hand om andra</h3>
                      <v-radio-group v-model="answer[7]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>9. Jag oroar mig ofta om vad andra tycker om mig</h3>
                      <v-radio-group v-model="answer[8]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>10. Jag vill ha så mycket stadga och trygghet i mitt liv som möjligt</h3>
                      <v-radio-group v-model="answer[9]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>11. Det är viktigt att bidra med samhällsnytta</h3>
                      <v-radio-group v-model="answer[10]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>12. Jag tycker om att utveckla nya idéer och projekt</h3>
                      <v-radio-group v-model="answer[11]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>13. Jag är väldigt riskmedveten</h3>
                      <v-radio-group v-model="answer[12]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>14. Jag är gärna en förebild för andra</h3>
                      <v-radio-group v-model="answer[13]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>15. Jag är en tävlingsmänniska</h3>
                      <v-radio-group v-model="answer[14]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>16. Jag avskyr känslan av att ha tråkigt</h3>
                      <v-radio-group v-model="answer[15]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>17. Jag har lätt för att skapa kontakt med andra</h3>
                      <v-radio-group v-model="answer[16]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>18. Jag försöker ständigt att förbättra mig själv</h3>
                      <v-radio-group v-model="answer[17]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>19. Fara är aldrig något spännande för mig</h3>
                      <v-radio-group v-model="answer[18]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>20. I mina nära relationer är jag oftast den som ger</h3>
                      <v-radio-group v-model="answer[19]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>21. Det finns alltid någonting nytt man kan lära sig</h3>
                      <v-radio-group v-model="answer[20]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>22. Jag måste känna mig tillfredsställd</h3>
                      <v-radio-group v-model="answer[21]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>23. Det är ofta jag betygsätter och bedömer mina egna prestation</h3>
                      <v-radio-group v-model="answer[22]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>24. Jag tycker om när man vet vad som ska hända</h3>
                      <v-radio-group v-model="answer[23]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>25. Jag är mer kärleksfull än de flesta</h3>
                      <v-radio-group v-model="answer[24]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>26. Att bli erkänd är viktigt för mig</h3>
                      <v-radio-group v-model="answer[25]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>27. Känslan av att något är ansträngande eller påfrestande tycker jag om</h3>
                      <v-radio-group v-model="answer[26]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>28. Jag är väldigt försiktig med utgifter</h3>
                      <v-radio-group v-model="answer[27]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>29. Utbildning är väldigt viktigt för mig</h3>
                      <v-radio-group v-model="answer[28]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>30. Jag är en ledare</h3>
                      <v-radio-group v-model="answer[29]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>31. Jag är söker alltid nya erfarenheter</h3>
                      <v-radio-group v-model="answer[30]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>32. Ibland överanstränger jag mig själv för att hjälpa andra</h3>
                      <v-radio-group v-model="answer[31]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>33. Mina rutiner och dagliga vanor är viktiga för mig</h3>
                      <v-radio-group v-model="answer[32]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>34. Jag är stolt över mig själv och den jag är</h3>
                      <v-radio-group v-model="answer[33]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>35. Jag tycker det är fantastiskt hur ens perspektiv förändrar sig när man lär sig något nytt</h3>
                      <v-radio-group v-model="answer[34]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>36. Ibland är det viktigaste arbetet något man inte får betalt för</h3>
                      <v-radio-group v-model="answer[35]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>37. Jag är inte en äventyrlig människa</h3>
                      <v-radio-group v-model="answer[36]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>38. Nej, jag skulle inte hävda att jag är självisk</h3>
                      <v-radio-group v-model="answer[37]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>39. Jag tenderar att göra av med mer än vad jag egentligen har</h3>
                      <v-radio-group v-model="answer[38]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>40. Jag tycker om att känna mig viktig</h3>
                      <v-radio-group v-model="answer[39]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>41. Varje misslyckande är en chans till ny lärdom.</h3>
                      <v-radio-group v-model="answer[40]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>42. Jag tycker om att lära mig nya saker för att själv kunna utbilda andra</h3>
                      <v-radio-group v-model="answer[41]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>43. Jag söker samförstånd i mina relationer</h3>
                      <v-radio-group v-model="answer[42]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>44. Jag tycker om att vara den som gör skillnad i sådant jag företar mig</h3>
                      <v-radio-group v-model="answer[43]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>45. Jag undviker att beblanda mig i saker om det inte redan finns ett säkert utfall</h3>
                      <v-radio-group v-model="answer[44]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>46. Jag lider när jag känner att jag inte kan eller får prestera till fullt ut</h3>
                      <v-radio-group v-model="answer[45]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>47. Ovisshet gör att jag njuter</h3>
                      <v-radio-group v-model="answer[46]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>48. Prestige är väldigt viktigt för mig</h3>
                      <v-radio-group v-model="answer[47]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>49. Jag är en romantisk person</h3>
                      <v-radio-group v-model="answer[48]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>50. Jag lär mig konstant nya saker</h3>
                      <v-radio-group v-model="answer[49]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>51. Det är viktigare för mig att kunna ge än att bara kunna ta</h3>
                      <v-radio-group v-model="answer[50]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>52. Jag vill alltid vara nummer ett</h3>
                      <v-radio-group v-model="answer[51]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>53. Jag avskyr att utsätta mig för risker</h3>
                      <v-radio-group v-model="answer[52]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>54. Jag vill ständigt utvecklas</h3>
                      <v-radio-group v-model="answer[53]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>55. Jag tycker om att lägga min tid och energi på goda ändamål</h3>
                      <v-radio-group v-model="answer[54]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>56. Jag tycker om när andra ser upp till mig</h3>
                      <v-radio-group v-model="answer[55]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>57. Jag är stolt över min förmåga att lära mig nya saker</h3>
                      <v-radio-group v-model="answer[56]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>58. Vi finns till för att göra världen till ett bättre ställe att vara på</h3>
                      <v-radio-group v-model="answer[57]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>59. Jag tycker om att utvecklas på många olika plan</h3>
                      <v-radio-group v-model="answer[58]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>60. Nära och personliga relationer är det absolut viktigaste i mitt liv</h3>
                      <v-radio-group v-model="answer[59]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>61. Ibland skrämmer min personlighet andra</h3>
                      <v-radio-group v-model="answer[60]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>62. Jag söker ständigt efter nya variationer i livet</h3>
                      <v-radio-group v-model="answer[61]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>63. Om något är riskfyllt oroar jag mig</h3>
                      <v-radio-group v-model="answer[62]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>64. Att jag själv är nöjd med mitt egna arbete är viktigare än att bli hyllad av andra</h3>
                      <v-radio-group v-model="answer[63]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>65. Jag strävar ständigt efter att förbättra mina egenskaper</h3>
                      <v-radio-group v-model="answer[64]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>66. Jag kommer andra nära genom att vara generös med pengar, tid och energi</h3>
                      <v-radio-group v-model="answer[65]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>67. Jag överväger gärna länge innan jag beslutar mig för att agera</h3>
                      <v-radio-group v-model="answer[66]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>68. Fara får mig ibland att rysa till av spänning</h3>
                      <v-radio-group v-model="answer[67]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>69. Jag måste känna mig respekterad</h3>
                      <v-radio-group v-model="answer[68]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>70. Om vi slutar att utvecklas som människa, så ”dör” vi inombords</h3>
                      <v-radio-group v-model="answer[69]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>71. Gemenskap är viktigt för mig</h3>
                      <v-radio-group v-model="answer[70]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>72. För att livet ska betyda något, måste man lämna sitt avtryck i världen</h3>
                      <v-radio-group v-model="answer[71]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>73. Att känna mig väl till lags är väldigt viktigt för mig</h3>
                      <v-radio-group v-model="answer[72]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>74. Jag tycker om att känna mig involverad i många aktiviteter</h3>
                      <v-radio-group v-model="answer[73]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>75. Jag jämför alltid min egen framgång med andras</h3>
                      <v-radio-group v-model="answer[74]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>76. Jag kräver passion i mina förhållanden</h3>
                      <v-radio-group v-model="answer[75]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>77. Om jag inte bidrar något till andra känns mitt liv meningslöst</h3>
                      <v-radio-group v-model="answer[76]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>78. När jag tar ett beslut väljer jag oftast alternativet som innebär minst friktion</h3>
                      <v-radio-group v-model="answer[77]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>79. Jag avskyr när saker och ting inte rör sig framåt</h3>
                      <v-radio-group v-model="answer[78]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>80. Jag måste känna mig trygg och säker så ofta som möjligt</h3>
                      <v-radio-group v-model="answer[79]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>81. Om jag bestämmer mig för något oroar jag mig för att jag kanske missar någonting annat</h3>
                      <v-radio-group v-model="answer[80]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>82. Jag vill aldrig uppfattas som en förlorare</h3>
                      <v-radio-group v-model="answer[81]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>83. Stabilitet i livet är inte så viktigt för mig</h3>
                      <v-radio-group v-model="answer[82]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                      <h3>84. Jag har ett kall, ett syfte i livet</h3>
                      <v-radio-group v-model="answer[83]" :mandatory="true">
                          <v-radio                            
                              label="ja"
                              :value="0"
                              :key="0"
                          ></v-radio>
                          <v-radio
                              label="delvis"
                              :value="1"
                              :key="1"
                          ></v-radio>
                          <v-radio
                              label="nej"
                              :value="2"
                              :key="2"
                          ></v-radio>
                      </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            

<!--
            <v-layout>
                <v-flex xs12 md6>
                    <v-text-field 
                        id="name"
                        :counter="30"
                        v-model="name"
                        label="namn"
                        required>
                    </v-text-field>
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-text-field 
                        id="price"
                        mask="####"
                        :counter="10"
                        v-model="price"
                        label="pris"
                        required>
                    </v-text-field>
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-text-field 
                        id="photo"
                        :counter="80"
                        v-model="photo"
                        label="fotolänk"
                        required>
                    </v-text-field>
                </v-flex>
            </v-layout>            
            <v-flex xs12 md6>
                <v-textarea
                    id="description"
                    name="input-7-1"
                    label="beskrivning"
                    v-model="description"
                    hint="Ingredienser, jämförelser, ursprung osv"
                    required>
                </v-textarea>
            </v-flex>
            <v-layout>
                <v-flex xs12 md6>
                    <v-text-field 
                        id="stock"
                        mask="######"
                        :counter="6"
                        v-model="stock"
                        label="antal i lager"
                        required>
                    </v-text-field>
                </v-flex>
            </v-layout>            
            <v-layout>
                <v-flex xs12 md6>
                    <v-container fluid px-0>
                    <v-radio-group v-model="group" :mandatory="true">
                        <v-radio                            
                            label="mat"
                            :value="0"
                            :key="0"
                        ></v-radio>
                        <v-radio
                            label="dryck"
                            :value="1"
                            :key="1"
                        ></v-radio>
                        <v-radio
                            label="övrigt"
                            :value="2"
                            :key="2"
                        ></v-radio>
                    </v-radio-group>        
                    </v-container>        
                </v-flex>
            </v-layout>            

            <p>Test for uploading images...</p>
            <v-flex xs12 md6>
                <img :src="imageUrl" height="150" v-if="imageUrl"/>
                <v-text-field label="Select Image" @click='pickFile' v-model='imageName' prepend-icon='attach_file'></v-text-field>
                <input
                    type="file"
                    style="display: none"
                    ref="image"
                    accept="image/*"
                    @change="onFilePicked"
                >
            </v-flex>
            -->
            <!--<v-btn v-on:click="addFormData()">INSERT FOOD</v-btn>-->
            <v-layout class="text-xs-right">
                <v-flex xs6 md6 >    
                    <v-btn v-on:click="addFood({id, name, price, photo, description, stock, group})">se resultat</v-btn>
                </v-flex>
            </v-layout>            

        </v-form>
  </div>
  </v-app>
</template>

<script>

import { mapMutations, mapGetters } from 'vuex';

export default {
  //name: 'home',
    data() {
        return {
            answer: [85], 
        };
    },
    methods: {
        ...mapMutations ([
            //'addFood',
            //'increaseId',
        ]),
        submitResult() {
          // id is autoincremented
          // username
          // question_number - ignore
          // question_answer
          // axios post { username, answer[84] }
           
    },
        addFormData() {
            this.name = '';
            return 1;
        },
    },
    computed: {
        ...mapGetters ([
        ]),
    },

}
</script>

<style scoped>
  .home {
    text-align: left;
    padding: 10%;
  }
</style>