<template>
	<div>
		<b-navbar toggleable="lg" type="light" variant="info">
			<b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

			<b-collapse id="nav-collapse" is-nav>
			<b-navbar-nav>
				<b-nav-item href="/">Home</b-nav-item>
				<b-nav-item href="/about">About</b-nav-item>
				<b-nav-item href="/participation">Participation</b-nav-item>
				<b-nav-item href="/publications">Publications</b-nav-item>
				<b-nav-item href="/faq">FAQ</b-nav-item>
				<b-nav-item href="/contact">Contact</b-nav-item>
			</b-navbar-nav>

			<!-- Right aligned nav items -->
			<b-navbar-nav class="ml-auto">
			</b-navbar-nav>
			</b-collapse>
		</b-navbar>
	</div>
</template>