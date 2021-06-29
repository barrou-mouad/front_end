
<template>

<div class="container">
    <div class="row">
      <!-- jours -->
        <div class="col-3" ><select id="select" @change="show();getsalle()">
            <option :value="day.id" v-for="day in planing" :key="day.id">{{day.jour}}</option>
        
            </select>
            
            </div>
        <div class="col-3">
           <!-- modules -->
            <select >
            <option @change="show()" id="md" :value="j.id" v-for="j in modules" :key="j">{{j.intitule}}</option>
            </select>
        </div>
              <div class="col-3" >
                 <!-- heure_debut -->
                <select id="date" @change="getsalle()" >
            <option :value="ja" v-for="ja in jour" :key="ja">{{ja}}</option>
            </select>
        </div>
                     <div class="col-3" >
                        <!-- salle -->
                       <select>
            <option :value="s.id" v-for="s in salles" :key="s.id">{{s.intitule}}</option>
            </select>
        </div>
       
    </div>
<p>Stoop</p>



<div>
  <b-card no-body>
    <b-tabs card>
      <b-tab title="Tab 1" active>
        <b-card-text>Tab contents 1</b-card-text>
      </b-tab>
      <b-tab title="Tab 2">
        <b-card-text> <gestionet/></b-card-text>
      </b-tab>
          <b-tab title="Tab 3">
        <b-card-text> <gestionet/></b-card-text>
      </b-tab>
    </b-tabs>
  </b-card>
</div>
            </div>
</template>


