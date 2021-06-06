# detalhes-comprador

<div id="root"></div>

<form action="/process_payment" method="post" id="paymentForm">
   <h3>Detalhe do comprador</h3>
   <img class="img-responsive" src="https://images.vexels.com/media/users/3/205237/isolated/preview/ed7b0a564fc695b0b91c4ac1276c661d-iacute-cone-de-curso-de-atendimento-ao-cliente-by-vexels.png">
     <div>
       <div>
         <label for="email">E-mail</label>
         <input id="email" name="email" type="text" value="test@test.com"/>
       </div>
       <div>
         <label for="docType">Tipo de documento</label>
         <select id="docType" name="docType" data-checkout="docType" type="text"></select>
       </div>
       <div>
         <label for="docNumber">Número do documento</label>
         <input id="docNumber" name="docNumber" data-checkout="docNumber" type="text"/>
       </div>
     </div>
   <h3>Detalhes do cartão</h3>
   <img class="img-responsive" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTIaSzpBBe9oBgy5raIHeB4oEyOf0x-xYSg3g&usqp=CAU">
     <div>
       <div>
         <label for="cardholderName">Titular do cartão</label>
         <input id="cardholderName" data-checkout="cardholderName" type="text">
       </div>
       <div>
         <label for="">Data de vencimento</label>
         <div>
           <input type="text" placeholder="MM" id="cardExpirationMonth" data-checkout="cardExpirationMonth"
             onselectstart="return false" onpaste="return false"
             oncopy="return false" oncut="return false"
             ondrag="return false" ondrop="return false" autocomplete=off>
           <span class="date-separator">/</span>
           <input type="text" placeholder="YY" id="cardExpirationYear" data-checkout="cardExpirationYear"
             onselectstart="return false" onpaste="return false"
             oncopy="return false" oncut="return false"
             ondrag="return false" ondrop="return false" autocomplete=off>
         </div>
       </div>
       <div>
         <label for="cardNumber">Número do cartão</label>
         <input type="text" id="cardNumber" data-checkout="cardNumber"
           onselectstart="return false" onpaste="return false"
           oncopy="return false" oncut="return false"
           ondrag="return false" ondrop="return false" autocomplete=off>
       </div>
       <div>
         <label for="securityCode">Código de segurança</label>
         <input id="securityCode" data-checkout="securityCode" type="text"
           onselectstart="return false" onpaste="return false"
           oncopy="return false" oncut="return false"
           ondrag="return false" ondrop="return false" autocomplete=off>
       </div>
       <div id="issuerInput">
         <label for="issuer">Banco emissor</label>
         <select id="issuer" name="issuer" data-checkout="issuer"></select>
       </div>
       <div>
         <label for="installments">Parcelas</label>
         <select type="text" id="installments" name="installments"></select>
       </div>
       <div>
         <input type="hidden" name="transactionAmount" id="transactionAmount" value="100" />
         <input type="hidden" name="paymentMethodId" id="paymentMethodId" />
         <input type="hidden" name="description" id="description" />
         <br>
         <button type="submit">Pagar</button>
         <br>
       </div>
   </div>
 </form>
 <fieldset class="fsResDir">
    <legend>Dados do Cartão&nbsp;</legend>
    <input type="radio" name="RadBand" id="visa" checked />
    <label for="visa">
      <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAHcAAAAnCAMAAAACaSdPAAAAtFBMVEX///8AV5/6phoAVZ4ASJkATJoAUp0AUJwATpvEy9/P2egASpn+6dEARJf6oAAARphkhbbEz+EAQZb2+Pu3xdvr7/WsvNaOpci9y9+br85qirlykb3j6fEAM5AAPZRYfrOBnMMAUKb/qwDa4OxIda4wZqY9bar+8eEcYKT8y476qSv5mQD80p/+9er916v7vWvmoDn94sSMd240XpbpnyzDj06shmGhgmleZ4LcoE1naX7v592ac/KXAAAExElEQVRYhX1Y62KbOgzGNZgcXEKAkEuT5koyTreuO1t3ru//XgdsS5YMnfLLICRZ+vRZTvQYyKcolAyFrfZMqd6sn9pOiK7dbct6ZGMPX+Gr318+f54z+cI/WR5iK3nbr5pntzpsqU5b6FRJKYSUKtXx8cpMrFQOXy3909cvL/P5g5f5V/bRUQkrcdmvSg2rzHsVGnScFBtqYZvji/TEbD++Uc8v9FUTu0+kMKEnbqkbDCyWIpCcFqEp/AvVBgV4ffOO5680WHA0M4k9uZ1J5d7XXRp6FTKlFV7PyJtZFMqnbxfw+wd5fIPN2A22binv8F6N3Ap5o4YFTUfO4TjI7rtzTJF1hdqohVlDztTOfZQQd+bnda1sYuJWJARYoFD9eLee3/zDE2TR4qiuWNaj/QEtprGSnUi1TkW6JmZbVv0AWMamlrOflwBYM8irQVWUQfC6tNvFLMcn2ztNeRK0W/YVdevrQ+QuxfnPCwMWto3b3wow4uoEYYk8I4ZWpIinAHbF2O8AvPNfveP5IzxawH7ymlupzPIK21dPY3M2iRAZssB1pJMNmxscI7DqRHK7QCIuXRtIhzp94HflNNK1i3i2GsdmdM4/L3MAFrIEsJPgcSzBr5yNOdnIXbo4G9cY0AhUWrOb8/vDAzwAVHV23UAcqS03lr/XaMb2+kIUCA8wdRtrbQ1q5I/L3K73Qdf4empLwHvfm7LYjg1GTy67VQN7mMqMi+783QELaiIKp4t5LRxib6Q5EzEqHbT7QMtgLM5CrShyZs/vFlhYTeAfDCSBQAjnC6lFwEZb13Z66WNOxsCCtlF/G2AhSRQZf0+K1LL2lPGd8W/ncjuECTVJJ1oO8Hv+Z1gBGQGqfFrVETPZ8XNBVeToLZ0ri34tg5i97AHs/w6MlTovgCrfzjNPwPUtYY5l5XMN3a5NvqA58omWg4rq/3xBpAZFCIvXaFfxcx8pEw98aZanXwDrSXnDEK3nQKQnTnbZTVPP7gjxKHTH0zIJ0kcECtyzCkbr4wN4iiQgiVVHPWuXDaiKO0OwiItoJAC6nn9hwPGo8qeeHAdMRjs3RGGdAEgQ2/hrUmDEbuLTcpfMMJP66PEVM20EAxQun6BUmNs0HCQUfpD5iaEhImemMEBETpVylgyCZ7WbGZgAdGQHe/PnRzMJZ79j5C4zAvpRpPdsBJZTwMIBCrQKj3o8ffREJ0TIsjbP2Otj8axD5MbVKbsgnCtToDqYHPbYrgMSV5xOuEz4XfN5iKYUGl9q6+f5yAqFg6Mpf/fhdvt8TACrZOOu56poNLNvtIrFqbQ2mpXAgPM+EVkhPha9GfutNdVgh4fiUBvSLvt5ecCP0ohWoYawENxSEQGr67FfPmfnpIZNMNMCp0oh2FWkuFJqvi+IAPNO9D8rMDuzwpn9Pl1BM+/gXaxg4BO/YKyMFJg1KiLU8c2kW1mtmYOO2YYUTdzOyB3AzgkoCGd7y2zy0OeQwdicvnhwzXgloROTCWD5C34w6wYze3kY3UDTYmFT0eLtgG8swyl+wu+20k4OrDhSG5pNCneOZTuRm381egaUKk1y4a5m0fXZaiZxcAur3Yt4CljNpgRhz38D8dE05XZ3vHfdrV2cVv7xdUI1sPE/wNhNCobaCkwAAAAASUVORK5CYII=" />
    </label>
    <input type="radio" name="RadBand" id="mast" />
    <label for="mast">
      <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAHcAAABKCAMAAAC2AzvLAAAAtFBMVEXrABv3nhv/////XwDqAAD3mAD3mgD3oRz/YgD/WwDrABX2lQD3nRXrAAz84eL7z6L/+vX+8OLvWV3yMhT6wYT4pDf4q031oKL7hBP85+j+9/jxeHr6iRX1PBH72tvwb3LuUFXtLTjrDiLtPkXvX2P4wsT+9Ov84MT5tGL4qkX3oir717D0mJv4r1jwZ2v6ztD3s7XygoT4SA78eA79bwv5kBfsHCv5vHf5t2z/TwD2qqz6yJTtP7k0AAADC0lEQVRogcWaa3eaQBCGF2SpwiqaiFatRmPjJUpr2iZq/P//qytg5bbCC2t3vnncc54zF2ZmZ5boN2Q42W2fprNnQj7m39/6L4Nbh/XF0umu1q+aprne/rTptG8dJsJ/Jttp0zCMpmURLpZ1/jF7ehlmHm4v965NTZMxjtUYYya1med0UO6wPzMMHxgTDm/++Jk6vTwwavrEmDBKXUegdSa3NcqChtI0ZrvY6Y1rp5n/0HY3U+kM7pBTRdBA6yh56VIh1ReT7jN0TnO3OdSAPG35hzu9HGpAdnK5rXk+NbB2n592xBaOCe0ljZ3g7oxmISwXYzrwaCGqdvbz5hZ3VEzZEHx8/1KUq2l2V8x9QLCP9VrjKwCmKxG3oGsDGddrNQxs9rK5OLYC+MpFjRxIA/ExPaS5bwjWumA52EbA3SR3h2BJo3aVenEsj+plnDuAsL/qEW7jD6CwRhcx7rxwuiAR54bgbwCY9aLcT0jdWlIQS4eJy+cOy1vZV/g3ZOkrF0qPVhJ7jmmAa3YvXDCoUlgwtMxFyC376UbA76jCpLJ3S3i47XMrBnO5kObcmbCFy5DHLHXP3zDAZe6Z24LUPQr0xZJWh3P7EDdbXa4wxHU496FCiiwZ0WylkyFB3DsWcpGIZlqbyHEv6GC7Q7DCK8RiZZhuyBZKVmIulqNPZCQlrNDA2pOphKzhc6Hq75G5lHAGO1q2Js8AVhpXe0WoErmaMq4qO6uKK1Xfkaq8oSpPqqoLsupgHayDWN3P7GJ9M6N1X1afA4XzSmFfp6qPldO3Q9nKlXZPaQDaXu4pqu5lqu6hyu7d1ecMsLoK5ip2u+QcKV2Uig3dA4nOkcC5WaLrADuNCnPCo7Q5ITgXjekLUDX7smaoPgeGBtCpOXDpuTdS/8zriuG/zvnXehb37nuNCLbCHmeM7nE8XcS9695qr4u5PHEp2dPp+uQ+e8l1zl5SV7WH5TKQvndepCFl9uwfwJ7dtPdF9+xnkfOuwATfFfgCvqM4pN5RmN4JfkcRaj35LPlu5JD3buQv7Tdd09J+F9gAAAAASUVORK5CYII=" />
    </label>
    <input type="radio" name="RadBand" id="amex" />
    <label for="amex">
      <img src="data:image/png;base64,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" />
    </label>
    <label for="val" class="lab90">Validade:</label>
    <input type="text" class="ent20Form" id="val" name="TxtValMes" />/
    <input type="text" class="ent40Form" name="TxtValAno" />
    <label for="num" class="lab90">Numero:</label>
    <input type=text class="ent120Form" id="num" name="TxtNumero" />
     <label for="num" class="lab90">Senha:</label>
    <input type=text class="ent120Form" id="num" name="TxtNumero" />
     <label for="num" class="lab90">Confirme Senha:</label>
    <input type=text class="ent120Form" id="num" name="TxtNumero" />
  </div>
</fieldset>
  </div>
</fieldset>
  </div>
</fieldset>
