<style>
/* 1) Center the layout container, not the text */
.inner {
  max-width: 670px !important;   /* pick 1200/1400/etc */
  width: 100% !important;
  margin-left: auto !important;
  margin-right: auto !important;
  display: block !important;       /* ensures auto margins work */
}

/* 2) Make sure text remains left-aligned */
body, #main_content_wrap, #main_content, .inner {
  text-align: left !important;
}

/* 3) (Optional) Responsive images that don’t force centering via text-align */
img {
  display: block;
  max-width: 100%;
  height: auto;
  margin: 10px auto;               /* center the image box itself; change to 0 if you prefer left */
}
</style>


<style>
/* Mobile fixes */
@media (max-width: 600px) {
  /* 1) Let the container breathe on phones */
  .inner {
    max-width: 100% !important;
    padding-left: 14px !important;
    padding-right: 14px !important;
  }

  /* 2) Make text/links wrap instead of overflowing */
  .paper-title-container,
  #abs0, #abs1, #abs2, #abs3, #abs4,       /* your abstract blocks */
  .abs, .abstract,                          /* future-proof selectors */
  p, li, h1, h2, h3, h4, h5, h6,
  a {
    overflow-wrap: anywhere;
    word-break: break-word; /* backup for older browsers */
    hyphens: auto;
  }

  /* 3) Keep images inside the viewport */
  img {
    max-width: 100% !important;
    height: auto !important;
  }

  /* 4) Make code blocks wrap instead of horizontal scrolling off-screen */
  pre, code {
    white-space: pre-wrap;    /* wrap long lines */
    word-break: break-word;
  }

  /* 5) Tables should scroll horizontally instead of breaking layout */
  table {
    display: block;
    width: 100%;
    overflow-x: auto;
  }
}
</style>


<style>
/* Safety net: never allow sideways scrolling */
html, body { overflow-x: hidden; }

/* Make padding count toward width calculations */
*, *::before, *::after { box-sizing: border-box; }

/* Mobile fixes */
@media (max-width: 600px) {
  /* Use full width with comfy side padding */
  .inner {
    max-width: 100% !important;
    min-width: 0 !important;             /* override theme's min-width */
    padding-left: 14px !important;
    padding-right: 14px !important;
  }

  /* Hide absolute-positioned decorations that can poke past the edge */
  #downloads,
  #forkme_banner {
    display: none !important;
  }

  /* Force long content to wrap instead of pushing the layout wide */
  .paper-title-container,
  #abs0, #abs1, #abs2, #abs3, #abs4,
  p, li, a, h1, h2, h3, h4, h5, h6 {
    overflow-wrap: anywhere;
    word-break: break-word;
    hyphens: auto;
  }

  /* Keep media within the viewport */
  img, iframe, video {
    max-width: 100% !important;
    height: auto !important;
  }

  /* Code and tables: don't shove the page sideways */
  pre, code {
    white-space: pre-wrap;
    word-break: break-word;
  }
  table {
    display: block;
    max-width: 100%;
    overflow-x: auto;
  }
}
</style>



<p align="center"> 
<img src="images/jy_2024.jpg" width="350">
</p>

**Email:** jeffrey.yang@eccles.utah.edu &nbsp;  **Office:** BUC 450B

**[Curriculum Vitae](CV_Jeffrey_Yang.pdf)**

<br>

### Job Market Paper


**[The Cost of Oversight: Hedge Fund Regulatory Risk and Market Efficiency](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5692322)** 
<button id="btn-abs0" onclick="toggleAbstract('abs0','btn-abs0')" 
  style="border:none; background:none; color:#0066cc; cursor:pointer; font-size:90%; margin-left:6px;">
  [+] Abstract
</button>  

<div id="abs0" style="display:none; margin:5px 0 10px 0;">
  <p>Regulators enforce rules to deter misconduct and maintain orderly markets. However, their task is complicated by hedge funds’ complex strategies, which are difficult to classify as legitimate or manipulative. Regulatory risk, the likelihood of investigation or litigation, deters manipulation but can also discourage legitimate trading. Thus, the net effect of regulatory risk on financial markets is an empirical question. This paper examines the impact of hedge fund regulatory risk on stock market efficiency. Increased regulatory risk hurts weak-form price efficiency and price informativeness, as hedge funds reduce informed trading in response. The results indicate that efficiency gains from deterring manipulation are outweighed by efficiency losses from reduced legitimate trading.
 </p>

</div>

<div style="height:0.5em;"></div>


### Working Papers

**[Does High Frequency Market Manipulation Harm Market Quality?](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4280120)** 
<button id="btn-abs1" onclick="toggleAbstract('abs1','btn-abs1')" 
  style="border:none; background:none; color:#0066cc; cursor:pointer; font-size:90%; margin-left:6px;">
  [+] Abstract
</button>  
with [Jonathan Brogaard](https://brogaard.utah.edu/) and [Dan Li](https://myweb.cuhk.edu.cn/lidan)  
_Revise and Resubmit, Review of Financial Studies_

<div id="abs1" style="display:none; margin:5px 0 10px 0;">
  <p>
    Manipulation of financial markets has long been a concern. With the automation of financial markets, the potential for high frequency manipulation has arisen. Yet, such behavior is hidden within vast sums of order book data, making it difficult to define and to detect. We develop a tangible definition of one type of manipulation, spoofing. Using proprietary user-level identified order book data, we show the determinants of spoofing. Exploiting SEC Litigation Releases and lagged spoofing profitability as instruments, we show causal evidence that spoofing increases volatility and transaction costs, and decreases price efficiency. The findings indicate that spoofing harms market quality.
  </p>
</div>

---

**[Cross-Asset Liquidity Transmission](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4875686)** 
<button id="btn-abs2" onclick="toggleAbstract('abs2','btn-abs2')" 
  style="border:none; background:none; color:#0066cc; cursor:pointer; font-size:90%; margin-left:6px;">
  [+] Abstract
</button>  
with [Jonathan Brogaard](https://brogaard.utah.edu/), [Pei-Fang Hsieh](https://mx.nthu.edu.tw/~pfhsieh/), and [Jimmy Yang](https://business.oregonstate.edu/users/jimmy-yang)  

<div id="abs2" style="display:none; margin:5px 0 10px 0;">
  <p>
    We study cross-asset liquidity transmission using a proprietary dataset that tracks trader activity across multiple asset classes. We find that derivatives market makers’ hedging demand worsens liquidity in the stock market. We establish causality by exploiting an exogenous shock in hedging caused by increased options market making incentives. Market maker hedging transmits liquidity from derivatives to stocks, with trade imbalances driving hedging demand and causing asymmetric trading in the stock market. Hedging trades have permanent price impacts, indicating information transfer at the expense of stock market quality. Aggressive end-of-day hedging further consumes liquidity, consistent with its role in intraday momentum.
  </p>
</div>

---

**[Teams and the Homophily Trap: Evidence from Open Source Software](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5395207)** 
<button id="btn-abs4" onclick="toggleAbstract('abs4','btn-abs4')" 
  style="border:none; background:none; color:#0066cc; cursor:pointer; font-size:90%; margin-left:6px;">
  [+] Abstract
</button>  
with [Davidson Heath](http://davidsontheath.github.io/), [Nathan Seegert](http://www.nathanseegert.com/), and [Rob Wuebker](https://rwuebker.notion.site/RO-R-WU-K-R-f974e372aad24db1bea26d097f855033)  

<div id="abs4" style="display:none; margin:5px 0 10px 0;">
  <p>
    Many real-world teams—for example startups, scientific collaborations, and the open-source software community—form through self-selection rather than assignment. Yet most empirical research on team diversity and performance focuses on teams are already formed, or a field experiment where team members have been randomly assigned. This paper examines how diversity emerges and affects performance in endogenously formed teams using a panel of over 148,000 open source software project-years from GitHub. We document three main findings. First, homophily—the tendency to affiliate with similar others—drives team formation, resulting in widespread and persistent homogeneity in endogenously formed teams. Second, diversity improves project performance, with the greatest gains observed among teams that were initially homogeneous. Third, we empirically document the "homophily trap" in endogenously-formed teams, showing that the very mechanism that fosters early team emergence and cohesion inhibits a team's long-run performance by deterring outsider entry. Finally, we show that the coordination costs of diversity, two measures of team dysfunction—higher contributor exit and team fracture—arise primarily at high levels of heterogeneity. These results highlight a central tradeoff in team formation: early interpersonal fit may come at the expense of long-run adaptability and success.
  </p>
</div>

---

**[The Coevolution of Technology and Prices in Cryptocurrencies](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5426235)** 
<button id="btn-abs3" onclick="toggleAbstract('abs3','btn-abs3')" 
  style="border:none; background:none; color:#0066cc; cursor:pointer; font-size:90%; margin-left:6px;">
  [+] Abstract
</button>  
with [Ran Duchin](https://sites.google.com/view/randuchin) and [Da Huang](https://dahuang-finance.github.io/)  

<div id="abs3" style="display:none; margin:5px 0 10px 0;">
  <p>
    This paper studies the joint dynamics of cryptocurrency technology, returns, and labor markets for developers. We construct high-frequency measures of GitHub bug reports ("Technology Flaws") and code commits ("Technology Development") for major coins. The main results are twofold. First, a new Technology Flaw predicts a 7 bp drop in next-day returns without future reversals. Second, a 1% decrease in coin valuation leads to a 0.14% decrease in Technology Development labor. These findings suggest that technology is a fundamental factor in cryptocurrency prices, and that prices and technology development coevolve through a bidirectional feedback mechanism.
  </p>
</div>

<script>
function toggleAbstract(absId, btnId) {
  var abs = document.getElementById(absId);
  var btn = document.getElementById(btnId);
  if (abs.style.display === "none") {
    abs.style.display = "block";
    btn.textContent = "[–] Abstract";
  } else {
    abs.style.display = "none";
    btn.textContent = "[+] Abstract";
  }
}
</script>


<div style="height:0.5em;"></div>

### Teaching

FINAN 4030: Corporate Finance (sole instructor), Summer 2024 <br>
Average instructor rating: 5.87/6 (**[Teaching Evaluation](finan_4030_evals.pdf)**)

FINAN 7850: Advanced Empirical Asset Pricing (teaching assistant), Fall 2023/2024/2025



