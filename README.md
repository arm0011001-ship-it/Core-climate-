<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<title>ОБРАЗЕЦ — макет чека</title>
<style>
  body {
    background: #e8e8e8;
    font-family: Arial, Helvetica, sans-serif;
    display: flex;
    justify-content: center;
    padding: 40px;
  }
  .receipt {
    position: relative;
    width: 420px;
    background: #fff;
    border-radius: 16px;
    padding: 24px 28px;
    box-shadow: 0 4px 16px rgba(0,0,0,0.15);
    overflow: hidden;
  }
  .watermark {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%) rotate(-30deg);
    font-size: 48px;
    font-weight: bold;
    color: rgba(200,0,0,0.15);
    white-space: nowrap;
    pointer-events: none;
    user-select: none;
  }
  .header {
    display: flex;
    align-items: center;
    gap: 10px;
    margin-bottom: 16px;
  }
  .logo {
    width: 32px;
    height: 32px;
    background: #21A038;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #fff;
    font-weight: bold;
    font-size: 18px;
  }
  .bank-name {
    font-size: 18px;
    font-weight: bold;
    color: #21A038;
  }
  .title {
    font-size: 16px;
    font-weight: bold;
    margin-bottom: 4px;
  }
  .date {
    font-size: 13px;
    color: #666;
    margin-bottom: 16px;
  }
  .row {
    display: flex;
    justify-content: space-between;
    padding: 8px 0;
    border-bottom: 1px solid #eee;
    font-size: 14px;
  }
  .row:last-child {
    border-bottom: none;
  }
  .label {
    color: #666;
  }
  .value {
    font-weight: 500;
    text-align: right;
  }
  .amount {
    font-size: 22px;
    font-weight: bold;
    color: #000;
    margin: 12px 0;
  }
  .footer {
    margin-top: 20px;
    font-size: 11px;
    color: #999;
    text-align: center;
    border-top: 1px dashed #ccc;
    padding-top: 12px;
  }
</style>
</head>
<body>
  <div class="receipt">
    <div class="watermark">ОБРАЗЕЦ</div>

    <div class="header">
      <div class="logo">С</div>
      <div class="bank-name">СберБанк</div>
    </div>

    <div class="title">Перевод по номеру карты</div>
    <div class="date">26 сентября 2026, 10:31:33 МСК</div>

    <div class="amount">5 000 ₽</div>

    <div class="row">
      <span class="label">Кому</span>
      <span class="value">Khasanova Alina Rubinova</span>
    </div>
    <div class="row">
      <span class="label">Страна</span>
      <span class="value">Абхазия</span>
    </div>
    <div class="row">
      <span class="label">Сумма</span>
      <span class="value">5 000 ₽</span>
    </div>
    <div class="row">
      <span class="label">Комиссия</span>
      <span class="value">30 ₽</span>
    </div>
    <div class="row">
      <span class="label">Списано</span>
      <span class="value">5 000 ₽</span>
    </div>
    <div class="row">
      <span class="label">От кого</span>
      <span class="value">Ивора Б.</span>
    </div>
    <div class="row">
      <span class="label">Откуда</span>
      <span class="value">+ 8193</span>
    </div>

  </div>
</body>
</html>
