<template>
    <div class="pt-10 grid gap-5 grid-cols-1 md:grid-cols-2 xl:grid-cols-3">
        <NuxtLink class="work-focus" id="work9" to="/works/work9">
            <img class="" src="~/assets/image/works/work9/work9-2.jpg" alt="work9" />
            <img class="" src="~/assets/image/works/work9/work9-1.jpg" alt="work9" />
        </NuxtLink>
        <NuxtLink class="work-focus" id="work8" to="/works/work8">
            <img class="" src="~/assets/image/works/work8/work8-2.jpg" alt="work8" />
            <img class="" src="~/assets/image/works/work8/work8-1.jpg" alt="work8" />
        </NuxtLink>
        <NuxtLink class="work-focus" id="work7" to="/works/work7">
            <img class="" src="~/assets/image/works/work7/work7-2.jpg" alt="work7" />
            <img class="" src="~/assets/image/works/work7/work7-1.jpg" alt="work7" />
        </NuxtLink>
        <NuxtLink class="work-focus" id="work6" to="/works/work6">
            <img class="" src="~/assets/image/works/work6/work6-2.jpg" alt="work6" />
            <img class="" src="~/assets/image/works/work6/work6-1.jpg" alt="work6" />
        </NuxtLink>
        <NuxtLink class="work-focus" id="work5" to="/works/work5">
            <img class="" src="~/assets/image/works/work5/work5-2.jpg" alt="work5" />
            <img class="" src="~/assets/image/works/work5/work5-1.jpg" alt="work5" />
        </NuxtLink>
        <NuxtLink class="work-focus" id="work4" to="/works/work4">
            <img class="" src="~/assets/image/works/work4/work4-2.jpg" alt="work4" />
            <img class="" src="~/assets/image/works/work4/work4-1.jpg" alt="work4" />
        </NuxtLink>
        <NuxtLink class="work-focus" id="work3" to="/works/work3">
            <img class="" src="~/assets/image/works/work3/work3-2.jpg" alt="work3" />
            <img class="" src="~/assets/image/works/work3/work3-1.jpg" alt="work3" />
        </NuxtLink>
        <NuxtLink class="work-focus" id="work2" to="/works/work2">
            <img class="" src="~/assets/image/works/work2/work2-2.jpg" alt="work2" />
            <img class="" src="~/assets/image/works/work2/work2-1.jpg" alt="work2" />
        </NuxtLink>
        <NuxtLink class="work-focus" id="work1" to="/works/work1">
            <img class="" src="~/assets/image/works/work1/work1-2.jpg" alt="work1" />
            <img class="" src="~/assets/image/works/work1/work1-1.jpg" alt="work1" />
        </NuxtLink>
    </div>
</template>

<style lang="scss" scoped>
.emphasis{
    border-radius: 0.5rem;
    opacity: 1.0;
    filter: grayscale(0%);
    transition: .3s ease-in-out;
    &:hover {
        opacity: 0.5;
        // filter: grayscale(100%);
        // filter: drop-shadow(0 10px 8px rgb(0 0 0 / 0.08)) drop-shadow(0 4px 3px rgb(0 0 0 / 0.2));
    }
}

//---ver1---
.work-focus {
    //background-color: rgba(240, 0, 0, 0.5);
	position: relative;
	cursor: pointer;
    img {
        border-radius: 0.5rem;
    }
    img:nth-of-type(1) {
        position: relative;
    }
    img:nth-of-type(2) {
        position: absolute;
        top: 0%;
        opacity: 1;
        transition: .3s ease-in-out;
    }
    &:hover img:nth-of-type(2) {
        opacity: 0;
    }
}

// // ---ver2--- 
// // Need to specify the background image path separately for each image
// .work-focus {
//     //background-color: rgba(240, 0, 0, 0.5);
// 	background: url(~/assets/image/works/work3.jpg);
// 	border-radius: 0.5rem;
// 	//overflow: hidden;
// 	cursor: pointer;
//     img {
//         //position: absolute;
//         //top: 0%;
//         border-radius: 0.5rem;
//         opacity: 1;
//         transition: .3s ease-in-out;
//     }
//     &:hover img {
//         opacity: 0;
//     }
// }
</style>

<script>
export default {
  components: {},
  props: [],
  data () {
    return {
    }
  },
  computed: {
  },
  mounted () {
    console.log("Grid mounted...");
  },
  unmounted() {
    console.log("Grid unmounted...");
  },
  methods: {
  }
}
</script>