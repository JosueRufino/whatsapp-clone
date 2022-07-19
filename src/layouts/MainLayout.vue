<template>
  <q-layout view="lHh Lpr lFf">

    <q-drawer
      v-model="leftDrawerOpen"
      show-if-above
      bordered
      width="450"
    >
      <div class="flex justify-between items-center bg-secondary" style="height:10%; width:100%">
        <q-avatar size="xl" class="q-ml-md">
            <img src="https://scontent.flad1-1.fna.fbcdn.net/v/t39.30808-6/240660574_1883461295167402_5298256499620085799_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=174925&_nc_ohc=VPA_DdHdzwoAX9KnTGy&_nc_ht=scontent.flad1-1.fna&oh=00_AT9CFZ7Pjg9CE-Wplo6eDWYlf2GOcMGESwmNuUvnao9zeQ&oe=62DC4104">
        </q-avatar>
        <div class="q-gutter-xs">
          <q-btn round color="primary" icon="data_usage" flat text-color="grey"/>
          <q-btn round color="primary" icon="chat" flat text-color="grey"/>
          <q-btn round color="primary" icon="more_vert" flat text-color="grey"/>
        </div>
      </div>

      <div class=" flex q-mt-sm">
        <q-input
            outlined
            v-model="text"
            input-class=""
            dense
            placeholder="Pesquisar ou começar uma nova conversa"
            class="bg-secondary q-ml-md"
            style="width:380px;"
            flat
          >
            <template  v-slot:prepend>
              <q-icon name="search" />
            </template>
          </q-input>
          <q-btn round color="primary" icon="filter_list" flat text-color="grey"/>
      </div>
      <q-separator class="q-mt-sm"/>
       <q-list bordered padding separator>
          <q-item clickable v-ripple to="/chat">
            <q-item-section top avatar>
              <q-avatar>
                <img src="https://scontent.flad1-1.fna.fbcdn.net/v/t39.30808-6/292262196_776060460200572_2111516310484362117_n.jpg?stp=cp1_dst-jpg&_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=bAzaSdYd9FUAX-bOjJt&_nc_ht=scontent.flad1-1.fna&oh=00_AT96hFSRfx3dRamlQSyF27Bb-LwS5iXqvE6KnEeoc2nsAA&oe=62DC4FD1">
              </q-avatar>
            </q-item-section>

            <q-item-section>
             <q-item-label class="text-subtitle1">
                Honório Sousa ZUBÚ
                <q-icon name="sentiment_satisfied" color="yellow"/>
              </q-item-label>
              <q-item-label caption>Wy me trairam.</q-item-label>
            </q-item-section>

            <q-item-section side top>
              <q-item-label class="text-green" caption>19:01</q-item-label>
             <q-badge rounded color="green" label="1" />
            </q-item-section>
          </q-item>
          <q-item clickable v-ripple>
            <q-item-section top avatar>
              <q-avatar>
                <img src="https://scontent.flad1-1.fna.fbcdn.net/v/t39.30808-6/280342663_3175049429437488_6893571322626397789_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=174925&_nc_ohc=ylBCsMB-MXYAX-2-XKq&_nc_ht=scontent.flad1-1.fna&oh=00_AT_DyrBS0OVh780DUkcQiCp4xsqei6oCWYsznI3RrV5_cA&oe=62DC9455">
              </q-avatar>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-subtitle1">
                Patricio Wilder
                <q-icon name="computer" color="blue"/>
              </q-item-label>
              <q-item-label caption>Estuda typescript.</q-item-label>
            </q-item-section>

            <q-item-section side top>
              <q-item-label class="text-green" caption>20:30</q-item-label>
             <q-badge rounded color="green" label="1" />
            </q-item-section>
          </q-item>
          <q-item clickable v-ripple>
            <q-item-section top avatar>
              <q-avatar>
                <img src="https://scontent.flad1-1.fna.fbcdn.net/v/t39.30808-6/277309060_1661978104141138_8142316206742276940_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=G9GscEFRBEwAX_hWK-B&_nc_ht=scontent.flad1-1.fna&oh=00_AT8K2-ufdFRKP2a3u5n0htThtJixLLFq7FmET-ldo1wvkA&oe=62DBF519">
              </q-avatar>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-subtitle1">
                Momma
                <q-icon name="favorite" color="red"/>
              </q-item-label>
              <q-item-label caption>Fiz uma transferência de 30 mil.</q-item-label>
            </q-item-section>

            <q-item-section side top>
              <q-item-label class="text-green" caption>10:23</q-item-label>
             <q-badge rounded color="green" label="1" />
            </q-item-section>
          </q-item>
           <q-item clickable v-ripple>
            <q-item-section top avatar>
              <q-avatar>
                <img src="https://scontent.flad1-2.fna.fbcdn.net/v/t39.30808-6/287674400_171111858664916_5912805046318389200_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=1jDz-0Hy4KkAX9cyPkV&_nc_ht=scontent.flad1-2.fna&oh=00_AT_SyWY5bjHQknMKmF5xjNWpVxtcrLiFr6MpUsAkI7OoLw&oe=62DCF7B3">
              </q-avatar>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-subtitle1">
                Lúcio José
              </q-item-label>
              <q-item-label caption>Clona o twitter.</q-item-label>
            </q-item-section>

            <q-item-section side top>
              <q-item-label class="text-green" caption>19:23</q-item-label>
             <q-badge rounded color="green" label="6" />
            </q-item-section>
          </q-item>
          <q-item clickable v-ripple>
            <q-item-section top avatar>
              <q-avatar>
                <img src="https://scontent.flad1-1.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?_nc_cat=1&ccb=1-7&_nc_sid=7206a8&_nc_ohc=LrRkDSLbr7MAX_JQg69&_nc_ht=scontent.flad1-1.fna&oh=00_AT-_3yT29w_sigVztpNsytUphxE7zMSvxUfrgLdV1fDH0Q&oe=62FDE278">
              </q-avatar>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-subtitle1">
                Juliana Soba
                <q-icon name="favorite" color="red"/>
              </q-item-label>
              <q-item-label caption>
                <q-icon name="done_all" color="blue" size="xs"/>
                OK.
              </q-item-label>
            </q-item-section>

            <q-item-section side top>
              <q-item-label caption>21:45</q-item-label>
            </q-item-section>
          </q-item>
          <q-item clickable v-ripple>
            <q-item-section top avatar>
              <q-avatar>
                <img src="https://scontent.flad1-1.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?_nc_cat=1&ccb=1-7&_nc_sid=7206a8&_nc_ohc=LrRkDSLbr7MAX_JQg69&_nc_ht=scontent.flad1-1.fna&oh=00_AT-_3yT29w_sigVztpNsytUphxE7zMSvxUfrgLdV1fDH0Q&oe=62FDE278">
              </q-avatar>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-subtitle1">
                  Benilsom Cambanza
                <q-icon name="favorite" color="red"/>
              </q-item-label>
              <q-item-label caption>
                <q-icon name="done_all" color="blue" size="xs"/>
                Estabilidade não existe, eu sempre te digo.
              </q-item-label>
            </q-item-section>

            <q-item-section side top>
              <q-item-label caption>21:45</q-item-label>
            </q-item-section>
          </q-item>

           <q-item clickable v-ripple>
            <q-item-section top avatar>
              <q-avatar>
                <img src="https://scontent.flad1-1.fna.fbcdn.net/v/t39.30808-6/280190620_3143962359264458_2966653292200022931_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=TfQRAdfZtwkAX8ie3cB&_nc_ht=scontent.flad1-1.fna&oh=00_AT8yE8_foTd44vLJ88CFDnCIzfo-8F3W7PjGontkXQAZ6w&oe=62DC943F">
              </q-avatar>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-subtitle1">
                  Nelma Valdez
                <q-icon name="favorite" color="red"/>
              </q-item-label>
              <q-item-label caption>
                Óla, moço.
              </q-item-label>
            </q-item-section>

            <q-item-section side top>
              <q-item-label caption>01:45</q-item-label>
            </q-item-section>
          </q-item>

          <q-item clickable v-ripple>
            <q-item-section top avatar>
              <q-avatar>
                <img src="https://scontent.flad1-1.fna.fbcdn.net/v/t39.30808-6/278811580_2057471094423702_634942747368382660_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=aaUlHcP3fFsAX-bQIBG&_nc_ht=scontent.flad1-1.fna&oh=00_AT8j08hoa9idtL44js0ox20b6YLeytus-wxNhDowRtZUeg&oe=62DC75C3">
              </q-avatar>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-subtitle1">
                  Lucas Pazito
                <q-icon name="favorite" color="red"/>
              </q-item-label>
              <q-item-label caption>
                Educar não é cortar as asas, mas sim orientar o voo.
              </q-item-label>
            </q-item-section>

            <q-item-section side top>
              <q-item-label caption>01:45</q-item-label>
            </q-item-section>
          </q-item>

          <q-item clickable v-ripple>
            <q-item-section top avatar>
              <q-avatar>
                <img src="https://scontent.flad1-1.fna.fbcdn.net/v/t39.30808-6/280190620_3143962359264458_2966653292200022931_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=TfQRAdfZtwkAX8ie3cB&_nc_ht=scontent.flad1-1.fna&oh=00_AT8yE8_foTd44vLJ88CFDnCIzfo-8F3W7PjGontkXQAZ6w&oe=62DC943https://scontent.flad1-1.fna.fbcdn.net/v/t39.30808-6/284689279_3142734906038845_8639394045893896898_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=Q0uOuGlbu2AAX8tdx0f&tn=IYMtPF6JkkWQMU7Y&_nc_ht=scontent.flad1-1.fna&oh=00_AT-p3-RwcOXkusGb91hbDcHQLizH-cRNWzBsGP7qxypRPg&oe=62DB7284F">
              </q-avatar>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-subtitle1">
                  Julio Dala
                <q-icon name="favorite" color="red"/>
              </q-item-label>
             <q-item-label caption>
                <q-icon name="done_all" color="blue" size="xs"/>
                Mana Pacha.
              </q-item-label>
            </q-item-section>

            <q-item-section side top>
              <q-item-label caption>01:45</q-item-label>
            </q-item-section>
          </q-item>
          
        </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>

</script>
