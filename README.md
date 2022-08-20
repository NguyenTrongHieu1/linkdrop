# LinkDrop contract

Confirm logic đã đọc - hiểu:
   	1> Build linkdrop.wasm voi file build.sh

	2> Login: near login

	3> Deploy: near deploy --accountId vnbc_hiu.testnet --wasmFile res/linkdrop.wasm --initFunction new --initArgs '{}'

	4> Kiểm tra keys: near keys vnbc_hiu.testnet

	5> Gọi hàm send 50 NEAR tới account phụ: vnbc_hiu2.testnet (có public_key:  ed25519:Gj8ximEYrb4EQYUUYn2vWHMYwJX14mqwbKFBA1yNonvG)
		: near call vnbc_hiu.testnet send '{"public_key": "ed25519:Gj8ximEYrb4EQYUUYn2vWHMYwJX14mqwbKFBA1yNonvG"}' --amount 50 --accountId vnbc_hiu.testnet --gas 300000000000000

	6> check self.accounts bằng hàm list_accounts '{}' do em tự viết 
		
	7> Kiểm tra lại keys của vnbc_hiu.testnet: near keys vnbc_hiu.testnet
		Có 1 Keys functionCall.
