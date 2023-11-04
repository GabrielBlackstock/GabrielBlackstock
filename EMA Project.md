```plaintext
//@version=5
indicator(title="Gabriel Crossover", shorttitle="Gabriel Crossover", overlay=true)
len5 = input.int(5, title="Fast Length", minval=1)
out50 = ta.ema(close, len5)
plot(out50, title="5 EMA", color=color.new(#00E676, 0), linewidth=1)

len10 = input.int(10, title="Fast Length", minval=1)
out10 = ta.ema(close, len10)
plot(out10, title="10 EMA", color=color.new(#FFEB3B, 0), linewidth=1)

len20 = input.int(20, title="Slow Length", minval=1)
out20 = ta.ema(close, len20)
plot(out20, title="20 EMA", color=color.new(#E040FB, 0), linewidth=1)

len40 = input.int(40, title="Slow Length", minval=1)
out40 = ta.ema(close, len40)
plot(out40, title="40 EMA", color=color.new(#311B92, 0), linewidth=1)


