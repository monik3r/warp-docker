Using `lanrat/wireguard-warp-generator` for docker containers.

Note that containers will use whatever networking is available as the warp config is allocated/brought up, so may leak initially.

We also patch out the DNS clause in the wireguard configs, so if you don't want to be leaking dns locally switch to the script under `/scripts/` in lanrat's repo.

Thanks lanrat, and thanks to cloudflare for this.
