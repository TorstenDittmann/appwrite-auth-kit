<div class="separator">or</div>

<style lang="scss">
	.separator {
		display: flex;
		align-items: center;
		text-align: center;
        width: 100%;
        font-size: 1.25rem;
        margin-top: 1.4rem;

		&:before,
		&:after {
			content: '';
			flex: 1;
			border-bottom: 1px solid lightgray;
		}

		&:not(:empty)::before {
			margin-right: 1em;
		}
		&:not(:empty)::after {
			margin-left: 1em;
		}
	}
</style>
