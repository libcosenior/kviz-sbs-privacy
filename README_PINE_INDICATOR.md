# Advanced S/R Zones Pine Script Indicator

## Popis / Description

Pokročilý Pine Script indikátor pre TradingView, ktorý kombinuje analýzu support/resistance zón s detekciou candlestick patterov a poskytuje komplexné obchodné signály s alertami.

Advanced Pine Script indicator for TradingView that combines Support/Resistance zone analysis with candlestick pattern detection and provides comprehensive trading signals with alerts.

## Vlastnosti / Features

### 1. Support/Resistance Zóny / Support/Resistance Zones
- ✅ **Optimalizovaný výpočet S/R zón** s nastaviteľnou citlivosťou
- ✅ **Vizualizácia pomocou boxov alebo čiar** (prepínateľné)
- ✅ **Výber timeframe** pre výpočet S/R zón
- ✅ **Automatické čistenie starých úrovní** pre výkon
- ✅ **Kompromis medzi presnosťou a rýchlosťou** - poznámky v kóde

### 2. Candlestick Patterns
- ✅ **Doji pattern** - detekcia nerozhodných sviečok
- ✅ **Harami pattern** - bullish a bearish varianty
- ✅ **Engulfing pattern** - pohltenie predchádzajúcej sviečky
- ✅ **Nastaviteľné threshold** pre Doji detekciu

### 3. Obchodné Signály / Trading Signals
- ✅ **BUY signály** - pri bullish patteroch blízko supportu
- ✅ **SELL signály** - pri bearish patteroch blízko resistance
- ✅ **Alerty pre BUY/SELL** signály
- ✅ **Automatické mazanie starých labelov**

### 4. Štatistiky / Statistics
- ✅ **Tabuľka so štatistikami** zobrazujúca:
  - Počet BUY signálov
  - Počet SELL signálov
  - Celkový počet signálov
  - Odhadovaný win-rate
  - Počet aktívnych S/R úrovní

### 5. Nastavenia / Settings
- 🎛️ **Support/Resistance nastavenia**
- 🎛️ **Pattern detekcia nastavenia**
- 🎛️ **Alert nastavenia**
- 🎛️ **Vizuálne nastavenia**
- 🎨 **Prispôsobiteľné farby**

## Inštalácia / Installation

1. Otvorte TradingView
2. Prejdite do Pine Editor (Alt + E)
3. Skopírujte obsah súboru `advanced_sr_indicator.pine`
4. Vložte do editora a stlačte "Add to Chart"

## Použitie / Usage

### Základné nastavenie / Basic Setup
1. **S/R Lookback Period**: 20 (štandardne) - počet sviečok pre hľadanie pivotov
2. **S/R Sensitivity**: 0.5 (štandardne) - nižšie hodnoty = viac úrovní
3. **S/R Timeframe**: prázdne (aktuálny timeframe) alebo špecifický timeframe

### Optimalizácia výkonu / Performance Optimization
- **Nižšia citlivosť** (vyššie S/R Sensitivity) = menej úrovní, rýchlejší výpočet
- **Vyššia citlivosť** (nižšie S/R Sensitivity) = viac úrovní, pomalší výpočet
- **Max S/R Levels**: limituje počet zobrazených úrovní

### Interpretácia signálov / Signal Interpretation
- 🟢 **BUY signál**: Bullish pattern blízko support úrovne
- 🔴 **SELL signál**: Bearish pattern blízko resistance úrovne
- 💎 **Doji**: Nerozhodnosť na trhu
- 🔺 **Harami**: Možný reversal pattern

## Kompromisy výkonu / Performance Trade-offs

| Nastavenie | Presnosť | Rýchlosť | Odporúčanie |
|------------|----------|----------|-------------|
| S/R Sensitivity 0.1-0.3 | Vysoká | Nízka | Pre swing trading |
| S/R Sensitivity 0.4-0.7 | Stredná | Stredná | **Odporúčané** |
| S/R Sensitivity 0.8-2.0 | Nízka | Vysoká | Pre scalping |

## Upozornenia / Warnings

⚠️ **Dôležité**: Indikátor je nástroj na analýzu, nie na automatické obchodovanie
⚠️ **Win-rate**: Aktuálne len odhad - pre presné meranie by bolo potrebné rozšírenie
⚠️ **Backtesting**: Odporúčame testovanie na historických dátach pred používaním

## Technické detaily / Technical Details

### Výkon / Performance
- **Maximálne boxy**: 100
- **Maximálne labely**: 50 (nastaviteľné)
- **Automatické čistenie** starých elementov
- **Pamäťová optimalizácia** pomocou arrays

### Algoritmus S/R
1. Výpočet pivot highs/lows
2. Filtrovanie podobných úrovní
3. Vizualizácia boxami alebo čiarami
4. Automatické čistenie starých úrovní

### Pattern detekcia
- **Doji**: Body < X% z celkového range
- **Harami**: Aktuálna sviečka v rámci predchádzajúcej
- **Engulfing**: Úplné pohltenie predchádzajúcej sviečky

## Changelog

### v1.0 (2024)
- ✅ Základná implementácia všetkých požadovaných funkcií
- ✅ S/R zóny s optimalizáciou
- ✅ Doji a Harami patterns
- ✅ BUY/SELL alerty
- ✅ Automatické čistenie labelov
- ✅ Timeframe výber
- ✅ Štatistická tabuľka

## Podpora / Support

Pre otázky a návrhy kontaktujte: libcosenior@gmail.com