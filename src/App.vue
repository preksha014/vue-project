  <script setup>
  // import { computed, reactive, ref, watch } from 'vue'
  import HelloWorld from './components/HelloWorld.vue'
  import Basics from './components/Basics.vue'

  // const firstName = "Preksha";

  // const lastName = "<p style=\"color:blue\">Rana</p>";

  // const objAttribute = {
  //   id: 'container',
  //   class: 'wrapper',
  //   style: 'background-color:pink; color:white; margin-top:5px;padding:10px; border-radius:10px;width:200px;'
  // };

  // const classObj = {
  //   active: true,
  //   'text-danger': false
  // };

  // const styleObj = {
  //   color: 'red',
  //   fontSize: '20px'
  // };

  // const obj = reactive({
  //   name: 'Preksha',
  //   age: 22,
  //   city: 'Delhi'
  // });

  // function showData() {
  //   obj.name = 'Prekshii';
  // };

  // const awesome = ref(true);

  // const parentMessage = ref('Parent')
  // const items = ref([{ message: 'Foo' }, { message: 'Bar' }])

  // const isPromoted = true;
  // const isSoldOut = false;

  // const isDisplay = true;

  // const names = ['Damon', 'Elena', 'Stefan', 'Caroline', 'Bonnie', 'Matt'];

  // const fullNames = [
  //   { name: 'Damon', surname: 'Salvatore' },
  //   { name: 'Elena', surname: 'Gilbert' },
  //   { name: 'Stefan', surname: 'Salvatore' },
  //   { name: 'Caroline', surname: 'Forbes' },
  //   { name: 'Bonnie', surname: 'Bennett' },
  //   { name: 'Matt', surname: 'Donovan' }
  // ];

  // const actors = [
  //   {
  //     name: 'Ian Somerhalder',
  //     series: ['The Vampire Diaries', 'Lost'],
  //   },
  //   {
  //     name: 'Nina Dobrev',
  //     series: ['The Vampire Diaries', 'Degrassi: The Next Generation'],
  //   }
  // ]

  // const count = ref(0);
  // const name = ref('Preksha');
  // function increment(num, event) {
  //   count.value++;
  //   console.log(event);
  // };
  // function decrement(num, event) {
  //   count.value--;
  //   console.log(event);
  // };

  // function changeName() {
  //   name.value = 'Prekshii';
  // }

  // const formValues = reactive({
  //   name: '',
  //   profileSummary: '',
  //   country: '',
  //   jobLocation: [],
  //   remoteWork: 'no',
  //   skillSet: [],
  //   yearsOfExperience: '',
  //   age: null,
  // });

  // function submitForm() {
  //   console.log(formValues);
  //   alert('Form submitted successfully!');
  // }

  // const products = reactive([
  //   {
  //     id: 1,
  //     title: 'TV',
  //     price: 100,
  //   },
  //   {
  //     id: 2,
  //     title: 'Phone',
  //     price: 200,
  //   },
  //   {
  //     id: 3,
  //     title: 'Laptop',
  //     price: 300,
  //   },
  // ]);

  // const total = computed(() => {
  //   return products.reduce((acc, item) => acc + item.price, 0);
  // });

  // const getExpensiveProducts = computed(() => {
  //   return products.filter((item) => item.price > 100);
  // });

  // const fullNameRef = ref('Preksha Rana');

  // function changeFullName() {
  //   fullNameRef.value = 'Het Shah';
  // }
  // const fullNameComputed = computed({
  //   get() {
  //     return `${fName.value} ${lName.value}`;
  //   },
  //   set(newValue) {
  //     const parts = newValue.split(' ');
  //     fName.value = parts[0] || '';
  //     lName.value = parts[1] || '';
  //   }
  // });

  // const volume = ref(0);
  // const movie = ref('Inception');
  // const movieInfo = reactive({
  //   title: 'Interstellar',
  //   actor: 'Matthew McConaughey'
  // });
  // const movieList = ref(['Avatar', 'Titanic']);

  // watch(volume, (newValue, oldValue) => {
  //   if (newValue > oldValue && newValue === 16) {
  //     alert('Listening to a high volume for a long time may damage your hearing');
  //   }
  // }, { immediate: true });

  // watch(movie, (newValue) => {
  //   console.log(`Calling API with movie name = ${newValue}`);
  // }, { immediate: true });

  // watch(movieInfo, (newValue) => {
  //   console.log(`Calling API with movie title = ${newValue.title} and actor = ${newValue.actor}`);
  // }, { immediate:true,deep: true });

  // watch(movieList, (newValue) => {
  //   console.log(`Updated list ${newValue}`);
  // }, { deep: true });

  const personName = 'Preksha Rana';
</script>

  <template>
    <!-- Text Interpolation -->
    <!-- <h1>Hello, <span>{{ firstName }}</span><span v-html="lastName"></span></h1> -->

    <!-- Boolean Attribute Binding -->
    <!-- <button :disabled="true">Click Me</button> -->

    <!-- Attribute Binding using object -->
    <!-- <div v-bind="objAttribute">Hello World!</div> -->

    <!-- Class and Style attribute binding using object -->
    <!-- <p :class="classObj" :style="styleObj">This is a paragraph</p> -->

    <!-- Event Handling -->
    <!-- <button @click="showData">Show Data</button>
    <p>{{ obj.name }} {{ obj.age }} {{ obj.city }}</p>

    <button @click="awesome = !awesome">Toggle</button> -->

    <!-- Conditional Rendering -->
    <!-- <h1 v-if="awesome">Vue is awesome!</h1>
    <h1 v-else>Oh no 😢</h1> -->

    <!-- List Rendering -->
    <!-- <li v-for="(item, index) in items" :key="index">
      {{ parentMessage }} - {{ index }} - {{ item.message }}
    </li>
    <br>
    <li v-for="(value, key) in obj" :key="key">{{ key }}:{{ value }}</li>
    <br> -->

    <!-- Binding Classes -->
    <!-- <p v-bind:class="isPromoted && 'promoted'">Promoted Movies</p>
    <p v-bind:class="isSoldOut ? 'sold-out' : 'new'">Sold Out Movies</p>
    <p v-bind:class="[isPromoted && 'promoted', isSoldOut ? 'sold-out' : 'new']">Promoted New Movies</p>
    <p v-bind:class="{
      'promoted': isPromoted,
      'sold-out': isSoldOut,
      'new': !isSoldOut
    }">Promoted New Movies</p> -->

    <!-- Conditional Rendering -->
    <!-- <template v-if="isDisplay">
      <h2>Preksha</h2>
      <h2>ranapreksha8@gmail.com</h2>
    </template> -->

    <!-- List Rendering -->
    <!-- <h3 class="list" v-for="name in names" :key="name">{{ name }}</h3><br>
    <h3 class="list" v-for="(fullName, index) in fullNames" :key="index">
      {{ fullName.name }} {{ fullName.surname }}
    </h3>

    <div class="list" v-for="(actor, index) in actors" :key="index">
      <h3>{{ actor.name }}</h3>
      <ul>
        <li v-for="(series, index) in actor.series" :key="index">{{ series }}</li>
      </ul>
    </div> -->

    <!-- Event Handling -->
    <!-- <p>{{ name }}</p>
    <p>{{ count }}</p>
    <button @click="changeName(), increment(1, $event)">Increment</button>
    <button @click="changeName(), decrement(1, $event)">Decrement</button> -->


    <!-- Form Handling -->
    <!-- <div>
      <pre>
    {{ JSON.stringify(formValues, null, 2) }}
  </pre>
    </div>
    <form @submit.prevent="submitForm">
      <div>
        <label for="name">Name</label>
        <input type="text" id="name" v-model.trim.lazy="formValues.name" />
      </div>
      <div>
        <label for="profile">Profile Summary</label>
        <textarea id="profile" v-model="formValues.profileSummary" />
      </div>
      <div>
        <label for="country">Country</label>
        <select id="country" v-model="formValues.country">
          <option value="">Select a country</option>
          <option value="india">India</option>
          <option value="vietnam">Vietnam</option>
          <option value="singapore">Singapore</option>
        </select>
      </div>
      <div>
        <label for="job-location">Job location</label>
        <select id="job-location" v-model="formValues.jobLocation" multiple>
          <option value="india">India</option>
          <option value="vietnam">Vietnam</option>
          <option value="singapore">Singapore</option>
        </select>
      </div>
      <div>
        <input id="remoteWork" type="checkbox" v-model="formValues.remoteWork" true-value="yes" false-value="no" />
        <label for="remoteWork">Open to remote work?</label>
      </div>
      <div>
        <label>Skill set</label>
        <input type="checkbox" id="html" value="html" v-model="formValues.skillSet" />
        <label for="html">HTML</label>
        <input type="checkbox" id="css" value="css" v-model="formValues.skillSet" />
        <label for="css">CSS</label>
        <input type="checkbox" id="javascript" value="javascript" v-model="formValues.skillSet" />
        <label for="javascript">JavaScript</label>
      </div>
      <div>
        <label>Years of Experience</label>
        <input type="radio" id="0-2" value="0-2" v-model="formValues.yearsOfExperience" />
        <label for="0-2">0-2</label>
        <input type="radio" id="3-5" value="3-5" v-model="formValues.yearsOfExperience" />
        <label for="3-5">3-5</label>
        <input type="radio" id="6-10" value="6-10" v-model="formValues.yearsOfExperience" />
        <label for="6-10">5-10</label>
        <input type="radio" id="10+" value="10+" v-model="formValues.yearsOfExperience" />
        <label for="10+">10+</label>
      </div>
      <div>
        <label for="age">Age</label>
        <input @keyup.enter="submitForm" type="number" id="age" v-model.number="formValues.age" />
      </div>
      <div>
        <button>Submit</button>
      </div>
    </form> -->

    <!-- Directive -->
    <!-- <button v-once @click="name = 'changedName'">{{ name }}</button>

    <p v-pre>{{ name }}</p> -->


    <!-- Computed Properties -->
    <!-- <p>{{ total }}</p>

    <button @click="products.push({ id: 4, title: 'Tablet', price: 400 })">Add Product</button> -->

    <!-- <template v-for="product in products" :key="product.id">
      <p v-if="product.price > 100">{{ product.title }} - {{ product.price }}</p>  
    </template> -->

    <!-- <p v-for="product in getExpensiveProducts" :key="product.id">
      {{ product.title }} - {{ product.price }}
    </p>

    <button @click="changeFullName">{{ fullNameRef }}</button>

    <div>
      <p> Current volume is :{{ volume }}</p>
      <div>
        <button @click="volume += 2">Increase</button>
        <button @click="volume -= 2">Decrease</button>
      </div>
    </div>

    <div>
      <input type="text" v-model="movie" />
      <p>Movie name is: {{ movie }}</p>

      <input type="text" v-model="movieInfo.title" placeholder="Movie Title" />
      <input type="text" v-model="movieInfo.actor" placeholder="Movie Year" />

      <button @click="movieList.push('Lost')">Add Movie</button>
    </div> -->

    <!-- Components -->
    <HelloWorld :personName="personName" />

    <Basics/>
  </template>

<style scoped>
/* .promoted {
  color: green;
  font-size: 20px;
}

.sold-out {
  color: red;
  font-size: 20px;
}

.new {
  font-style: italic;
  font-size: 20px;
}

.list {
  list-style-type: none;
  padding: 5px;
  margin: 5px;
  font-size: 20px;
  font-weight: bold;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

label {
  font-weight: bold;
  display: flex;
  margin-bottom: 5px;
}

input+label {
  font-weight: bold;
  display: inline-flex;
  margin-right: 20px;
}

input[type='text'],
textarea,
select {
  display: block;
  width: 400px;
  padding: 6px 12px;
  font-size: 14px;
  line-height: 1.42857143;
  color: #555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 4px;
} */
</style>
