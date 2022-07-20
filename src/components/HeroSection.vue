<template>
<div id="nav">



<div class="container overflow-hidden p-0">
	<div class="row g-0">
		<div lc-helper="background" class="col-md-6 order-md-2" style="min-height: 50vh; max-height: 90vh;background-size: cover; background-position: center; background-image: url('https://images.unsplash.com/photo-1488282396544-0212eea56a21?ixlib=rb-1.2.1&amp;q=80&amp;fm=jpg&amp;crop=entropy&amp;cs=tinysrgb&amp;w=1080&amp;h=768&amp;fit=crop&amp;ixid=eyJhcHBfaWQiOjM3ODR9');">

		</div>
		<div class="col-md-6 order-md-1 my-auto text-center" style="padding:10vw">

			<div class="lc-block mb-3">
				<div editable="rich">
					<h2>Hello World!</h2>
					<p class="lead">Lorem ipsum dolor sit amet, consectetur adipiscing</p>

				</div>

			</div>

			<div class="lc-block">
				<a class="btn btn-primary" href="#" role="button">Click me, I'm a button</a>
                <p>Social media icons</p>
                
			</div><!-- /lc-block -->

		</div>
	</div>
</div>

</div>
</template>
<script>
export default {
    name: "HeroSection",
    data() {
        return {
            title: "Hello nav"
        }
    }
}
</script>
<style>

</style>