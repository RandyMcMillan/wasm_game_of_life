default:
	. ~/.nvm/nvm.sh && nvm use && nvm exec yarn add npm-cli || yarn add npm-cli
	hash rustup || curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh && \
		rustup default nightly
	wasm-pack build || cargo install cargo-generate && cargo install wasm-pack
	yarn init wasm-app www && \
		cd www && yarn && yarn run start & source ./open && o http://localhost:8080

