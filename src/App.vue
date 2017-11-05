<template>
	<div class="app">
		<div class="browser-modal">
			<header>
				<p class="title">You seem to be using an unsupported browser</p>
			</header>
			<p class="description">
				To get the most out of using the new Return Path
			</p>
			<p class="description no-margin">
				please login to the new experience with a supported browser.
			</p>
			<div class="browser-list">
				<div class="browser-item">
					<chrome-svg />
					<p class="browser-name">Chrome</p>
				</div>
				<div class="browser-item">
					<safari-svg />
					<p class="browser-name">Safari</p>
				</div>
				<div class="browser-item">
					<firefox-svg />
					<p class="browser-name">Firefox</p>
				</div>
				<div class="browser-item">
					<ie-svg />
					<p class="browser-name">IE 11</p>
				</div>
				<div class="browser-item">
					<opera-svg />
					<p class="browser-name">Opera</p>
				</div>
			</div>
			 <div class="browser-action">
				 <button class="btn">Got it</button>
			</div>
		</div>
	</div>
</template>

<script>

import ChromeSvg from './components/Chrome';
import FirefoxSvg from './components/Firefox';
import IeSvg from './components/Ie';
import OperaSvg from './components/Opera';
import SafariSvg from './components/Safari';

export default {
	name: 'app',
	components: {
		ChromeSvg,
		FirefoxSvg,
		IeSvg,
		OperaSvg,
		SafariSvg,
	},
};
</script>

<style lang="scss" scoped>

.app {
	padding: 25vh 0;
}

.browser-action {
	margin-top: 45.1px;
	text-align: center;

	.btn {
		background-color: #105D7A;
		border-radius: 2px;
		border: 1px solid #25a0d4;
		color: #fff;
  	font-size: 12px;
  	font-weight: bold;
  	letter-spacing: 1.2px;
		padding: 8px 28px;
		text-transform: uppercase;
	}
}

.browser-modal {
  background-color: #fff;
  border-radius: 2px;
  box-shadow: 0 0 10px 0 rgba(63, 77, 89, 0.11);
	margin: auto;
	max-width: 470px;
	padding: 46px 48px 56px 48px;
}

.browser-list {
	display: flex;
	justify-content: center;
	margin-top: 33.9px;

	.browser-item {
		margin-right: 33.5px;
	}

	.browser-name {
  	color: #555555;
  	font-size: 10px;
		text-align: center;
	}

}

.title {
  color: #325e82;
  font-size: 16px;
  font-weight: 500;
  letter-spacing: 0.5px;
  line-height: 1.25;
  text-align: center;
}

.description {
  color: #325e82;
  font-size: 14px;
  font-weight: 300;
  line-height: 1.43;
  text-align: center;
}

.no-margin {
	line-height: 0;
	margin: 0;
}
</style>
