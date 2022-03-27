<template>
  <div class="wrapper" ref="aaaa">
    <ul class="zz">
      <button @click="btnClick"></button>
    <li>利润表1</li>
    <li>利润表2</li>
    <li>利润表3</li>
    <li>利润表4</li>
    <li>利润表5</li>
    <li>利润表6</li>
    <li>利润表7</li>
    <li>利润表8</li>
    <li>利润表9</li>
    <li>利润表10</li>
    <li>利润表11</li>
    <li>利润表12</li>
    <li>利润表13</li>
    <li>利润表14</li>
    <li>利润表15</li>
    <li>利润表16</li>
    <li>利润表17</li>
    <li>利润表18</li>
    <li>利润表19</li>
    <li>利润表20</li>
    <li>利润表21</li>
    <li>利润表22</li>
    <li>利润表23</li>
    <li>利润表24</li>
    <li>利润表25</li>
    <li>利润表26</li>
    <li>利润表27</li>
    <li>利润表28</li>
    <li>利润表29</li>
    <li>利润表30</li>
    <li>利润表31</li>
    <li>利润表32</li>
    <li>利润表33</li>
    <li>利润表34</li>
    <li>利润表35</li>
    <li>利润表36</li>
    <li>利润表37</li>
    <li>利润表38</li>
    <li>利润表39</li>
    <li>利润表40</li>
    <li>利润表41</li>
    <li>利润表42</li>
    <li>利润表43</li>
    <li>利润表44</li>
    <li>利润表45</li>
    <li>利润表46</li>
    <li>利润表47</li>
    <li>利润表48</li>
    <li>利润表49</li>
    <li>利润表50</li>
    <li>利润表51</li>
    <li>利润表52</li>
    <li>利润表53</li>
    <li>利润表54</li>
    <li>利润表55</li>
    <li>利润表56</li>
    <li>利润表57</li>
    <li>利润表58</li>
    <li>利润表59</li>
    <li>利润表60</li>
    <li>利润表61</li>
    <li>利润表62</li>
    <li>利润表63</li>
    <li>利润表64</li>
    <li>利润表65</li>
    <li>利润表66</li>
    <li>利润表67</li>
    <li>利润表68</li>
    <li>利润表69</li>
    <li>利润表70</li>
    <li>利润表71</li>
    <li>利润表72</li>
    <li>利润表73</li>
    <li>利润表74</li>
    <li>利润表75</li>
    <li>利润表76</li>
    <li>利润表77</li>
    <li>利润表78</li>
    <li>利润表79</li>
    <li>利润表80</li>
    <li>利润表81</li>
    <li>利润表82</li>
    <li>利润表83</li>
    <li>利润表84</li>
    <li>利润表85</li>
    <li>利润表86</li>
    <li>利润表87</li>
    <li>利润表88</li>
    <li>利润表89</li>
    <li>利润表90</li>
    <li>利润表91</li>
    <li>利润表92</li>
    <li>利润表93</li>
    <li>利润表94</li>
    <li>利润表95</li>
    <li>利润表96</li>
    <li>利润表97</li>
    <li>利润表98</li>
    <li>利润表99</li>
    <li>利润表100</li>
  </ul>
  </div>
</template>

<script>
import BScroll from "better-scroll"
export default {
  data() {
    return {
      scroll:null
    }
  },
  created() {
    // this.scroll=new BScroll(this.$refs.aaaa, {

    // })
  },
  mounted() {
    this.scroll=new BScroll(this.$refs.aaaa, {
      probeType:3,
      pullUpLoad:true
    })
    this.scroll.on('scroll',(position)=>{
      console.log(position);
    })
    this.scroll.on('pullingUp',()=>{
      console.log('上拉加载更多');
    })
  },
  methods: {
    btnClick() {
      console.log('btnClick');
    }
  },
}
</script>

<style scoped>
.wrapper {
  height: 150px;
  background-color: pink;
  overflow: hidden;
  overflow: scroll;
}
</style>
