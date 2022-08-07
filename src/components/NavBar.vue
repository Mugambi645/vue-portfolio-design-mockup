<template>


<section>
	<div class="container d-flex flex-wrap justify-content-between align-items-center py-3 my-4 border-bottom">
		<div class="col-md-4 d-flex align-items-center">
			<div class="lc-block text-center mb-3 mb-md-0">
				<a class="navbar-brand" href="https://library.livecanvas.com/sections/">
					<img class="img-fluid me-1" src="https://getbootstrap.com/docs/5.1/assets/brand/bootstrap-logo.svg" alt="my brand" width="48px" height="48px">
				</a>

				<span editable="inline" class="text-muted">Patrick Mugambi</span>

			</div>
		</div>


		<div class="col-md-4 justify-content-end d-flex gap-3">
			<div class="lc-block">
     <a
                class="nav-link"
                href="/resume"
                @click.prevent="$emit('scroll', 'resume')"
                :class="{ 'text-light': nightMode }"
                >Resume</a
              >
			</div>
			<div class="lc-block">

			<p>Portfolio</p>

			</div>
			<div class="lc-block">

			<p>About</p>

			</div>
            <div class="lc-block">

			<p>Contact</p>

			</div>
		</div>
	</div>
</section>


</template>
<script>
export default {
    name: "NavBar",
    data() {
        return {
            title: "Hello nav"
        }
    }
}
</script>
<style>

</style>