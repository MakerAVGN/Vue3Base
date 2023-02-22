<script>
export default {
  data() {
    return {
      hrefs: [
        { href: '1.html', text: 'text1' },
        { href: '2.html', text: 'text2' },
        { href: '3.html', text: 'text3' },
      ],
      products: [
        {
          name: 'product1',
          price: 100,
          quantity: 5
        },
        {
          name: 'product2',
          price: 200,
          quantity: 4
        },
        {
          name: 'product3',
          price: 300,
          quantity: 3
        },
      ]
    }
  },
  methods: {
  }
}
</script>
<template>
 <div class="a">
     <ul>
      <li v-for="href in hrefs">
        {{ href.href }}
        {{ href.text }}
      </li>
     </ul>
 </div>

<div class="b">
  <tr>
    <td v-for="text in products">
      {{ text.name }} <br>
      {{ text.price }} <br>
      {{ text.quantity }}
    </td>
  </tr>
</div>




</template>



