<template>
    <!-- <Pane title="Картографические материалы"  @close="$emit('close')"> -->
    <div>
        <LayerItem 
            class="item" 
            v-for="treeRoot in treeRoots" 
            :key="treeRoot.id" 
            :model="treeRoot" 
            :layers="layers" 
            ref="layeritem"
        ></LayerItem>
    </div>
    <!-- </Pane> -->
</template>

<script>
// import Pane from './Pane.vue'
import LayerItem from './LayerItem.vue'


export default {
  name: 'layers',
  components: { LayerItem },
  data () {
    return {
      treeRoots: null,
      layers: [],
    }
  },
  created () {
    const treeRoots = [
        {
            "name": "Административное устройство",
            "nodes": [
                {
                    "id": "148ac32a",
                    "name": "Административные центры районов",
                },
                {
                    "id": "5ba8149e",
                    "name": "Границы территорий",
                }
            ]
        },
        {
            "name": "ГИС. Документы",
            "nodes": [
                {
                    "id": "a161551f",
                    "name": "Зоны действия документов инженерных изысканий",
                },
                {
                    "id": "2bd50162",
                    "name": "Зоны действия документов",
                },
                {
                    "id": "14d1a142",
                    "name": "Разрешения на строительство",
                }
            ]
        },
        {
            "name": "ГИС. Зонирование территории ",
            "nodes": [
                {
                    "id": "a4e74133",
                    "name": "Зоны с особыми условиями использования территории",
                },
                {
                    "id": "6fb6d289",
                    "name": "Категории земель",
                },
                {
                    "id": "ea741c32",
                    "name": "Территориальные зоны Ленинградской области",
                },
                {
                    "id": "ebc0763e",
                    "name": "Функциональные зоны",
                },
                {
                    "id": "36d8002e",
                    "name": "СЗ зона",
                }
            ]
        },
    ]

    let layers = [
        {
            "id": "148ac32a",
            "name": "Административные центры районов",
        },
        {
            "id": "5ba8149e",
            "name": "Границы территорий ОКТМО Ленинградской области (служебный)",
        },
        {
            "id": "a161551f",
            "name": "Зоны действия документов инженерных изысканий ГИСОГД",
        },
        {
            "id": "2bd50162",
            "name": "Зоны действия документов",
        }
    ]

    this.layers = layers
    this.treeRoots = treeRoots
  },

}
</script>

