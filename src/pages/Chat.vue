<template>
    <q-page>
        <div class="flex justify-between items-center bg-secondary" style="height:10vh; width:100%">
            <div class="flex q-ml-md">    
                <q-item-section top avatar>
                <q-avatar>
                    <img src="https://scontent.flad1-1.fna.fbcdn.net/v/t39.30808-6/292262196_776060460200572_2111516310484362117_n.jpg?stp=cp1_dst-jpg&_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=bAzaSdYd9FUAX-bOjJt&_nc_ht=scontent.flad1-1.fna&oh=00_AT96hFSRfx3dRamlQSyF27Bb-LwS5iXqvE6KnEeoc2nsAA&oe=62DC4FD1">
                </q-avatar>
                </q-item-section>

                <q-item-section>
                <q-item-label class="text-subtitle1">
                    Honório Sousa ZUBÚ
                </q-item-label>
                </q-item-section>
            </div>

            <div side>
              <q-btn icon="search" flat/>
              <q-btn icon="more_vert" flat/>
            </div>

        </div>
        <div  style="height:80vh;padding-top:20px;background-image: url(https://i.pinimg.com/736x/8c/98/99/8c98994518b575bfd8c949e91d20548b.jpg);"> 
        <div class="q-ml-xl" style="width: 100%; max-width: 700px;background-image: url(https://i.pinimg.com/736x/8c/98/99/8c98994518b575bfd8c949e91d20548b.jpg);">
            <q-chat-message
                :text="['hey, how are you?']"
                sent
                stamp="7 minutos"
            />
            <q-chat-message
                :text="['doing fine, how r you?']"
                stamp="7 minutos"
            />
            <q-chat-message
                :text="['hey, how are you?']"
                sent
                stamp="7 minutos"
            />
            <q-chat-message
                :text="['doing fine, how r you?']"
                stamp="7 minutos"
            />
            <q-chat-message
                :text="['hey, how are you?']"
                sent
                stamp="7 minutos"
            />
            <q-chat-message
                :text="['doing fine, how r you?']"
                stamp="7 minutos"
            />
             <q-chat-message
                :text="['hey, how are you?']"
                sent
                stamp="7 minutos"
            />
            <q-chat-message
                :text="['doing fine, how r you?']"
                stamp="7 minutos"
            />
        </div>
    </div>
    <div class=" bg-secondary flex items-center" style="height:10vh; width:100%">
        <q-btn icon="sentiment_satisfied" color="grey" size="lg" flat/>
        <q-btn icon="attach_file" color="grey" size="lg" flat/>
        <q-input
            outlined
            v-model="text"
            dense
            placeholder="mensagem"
            class="bg-white q-ml-md"
            style="width:620px;"
            flat
          />
          <q-btn icon="mic" color="grey" size="lg" flat/>
    </div>
    </q-page>
</template>