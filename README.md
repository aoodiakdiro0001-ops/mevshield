# 🥪 MEVShield — MEV Risk & Gas Simulator (MIT)

Educational sandwich-risk analyzer, constant-product simulator and live
gas advisor. UI in EN/TR/AR. Static single file + README.
**Never sends transactions or moves funds.**

## Tools

- **🛡️ Risk Analyzer:** trade size, pool TVL, slippage, mempool visibility
  → 0–100 score + tier + 5 concrete defenses.
- **🥪 Simulator (x·y=k):** real AMM math with 0.3% fee — attacker sizes
  against YOUR slippage limit (tx reverts below minimum = nothing to steal).
  Shows optimal attacker size + net profit after gas.
- **⛽ Gas Advisor:** live `eth_gasPrice` + `eth_feeHistory` percentiles
  (publicnode) + CoinGecko prices; slow/std/fast/🚀-outrun tiers;
  maxFee = 2×base + priority; cost in USD.
- **🔒 Safe venues:** Flashbots Protect + MEV Blocker (official) + referral
  cards (`CONFIG.refs`: Binance + Pocket live).

## Money & contact

- `CONFIG.ads` footer slot (high-CPM crypto ads).
- Donate: BTC + USDT-TRC20 + IBANs.
- 📧 baranavisat@gmail.com · 📞 +90 531 326 37 22 · WhatsApp

## Run

```bash
cd mevshield
python3 -m http.server 8080
```

## License

MIT. Educational simulator — not financial advice.

## Telegram (@BaranScanBot)

- Footer'da herkese açık "Telegram" butonu (`t.me/BaranScanBot`) — ziyaretçi
  doğrudan bota yazar, ek ayar gerekmez.
- Sipariş/satış bildirimleri (`tgSend`) yalnızca `CONFIG`... `TG.chat`
  doluysa sahibine gider. Chat ID'yi @userinfobot'tan alıp `TG.chat`e yazın.
- ⚠️ **GÜVENLİK:** Bot tokeni herkese açık istemci kodundadır; kaynağı
  gören herkes bot adına mesaj gönderebilir. Kötüye kullanımda BotFather'dan
  tokeni yenileyin ve asla bu botla hassas işlem yapmayın. Gerçek çözüm:
  backend proxy.
