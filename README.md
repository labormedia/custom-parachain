# JIN PARACHAIN TESTNET

```bash
./target/release/parachain-template-node build-spec --disable-default-nodes > ../plain-parachain-chainspec.json
```

```bash
./target/release/parachain-template-node build-spec --chain plain-parachain-chainspec.json --disable-default-bootnode --raw > ../raw-parachain-chainspec.json
```

```bash
./target/release/jin-node     --alice     --collator     --force-authoring     --chain ../raw-parachain-chainspec.json     --base-path /tmp/collator_1     --port 40333     --rpc-port 8844     --     --execution wasm     --chain /GitHub/paseo-network/runtimes/chain-specs/paseo.raw.json     --port 30343
```
~
```bash
./target/release/jin-node     --bob     --collator     --force-authoring     --chain ../raw-parachain-chainspec.json     --base-path /tmp/collator_2     --port 40333     --rpc-port 8845     --     --execution wasm     --chain /GitHub/paseo-network/runtimes/chain-specs/paseo.raw.json     --port 30343 --rpc-port 9977
```
