
# My breakpoints-module - Itay Haephrati

### Enhanced Breakpoint Management for Responsive Web Design

Welcome to the streamlined and intuitive breakpoint system tailored for today's multi-device world. This repository offers a simple yet efficient system for managing breakpoints using SASS mixins. By establishing a coherent set of breakpoints, designers and developers can build websites that effortlessly adapt across a multitude of devices.

**Features:**

-   Defined standard breakpoints catering to modern screen sizes.
-   Use of SASS mixins for precise and clear implementation.
-   Flexibility to define styles from mobile-only to specific device sizes like iPad.

Stay ahead of the curve and ensure your website looks stunning, irrespective of the device it's viewed on.

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
