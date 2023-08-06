# My breakpoints-module - Itay Haephrati

// Using CSS variables
@import './assets/styles/breakpoints.module.scss';

:root {
	--primary: #0daec9;
	--primary-dark: #068298;
	--surface: #181d1f;
	--max-width: #{$xlBreakpoint};
}



// General use

@import 'breakpoints.module.scss';
.cardWrapper {
	width: 100%;
	@include min-md {
		width: calc((100% - rem(32px)) / 3);
	}
}
