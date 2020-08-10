---
layout: default
title: Asic Product
permalink: /asic
---
<div class="row asic">
    <p class="head">asic product</p>
    <p class="name">CoolDoG 001</p>
    <img src="/assets/img/cooldog_01.png" />
    {% assign cooldog = site.data.cooldog %}
    <table style="border: 0px; width:803px; margin: 0 auto;">
        <tr class="item">
            <td class="title">Technology</td><td colspan="4">{{ cooldog[0].technology }}</td>
        </tr>
        <tr class="item">
            <td class="title">Power Dissipation</td><td colspan="4">{{ cooldog[1].power }}</td>
        </tr>
        <tr class="item">
            <td rowspan="4" style="border-bottom: 1px #D8D8D8 solid;">Hashrate</td>
            <td class="attr">Algorithm</td>
            {% for algo in cooldog[2].algo %}
            <td>{{ algo }}</td>
            {% endfor %}
        </tr> 
        <tr class="item">
            <td class="attr">Asset</td>
            {% for asset in cooldog[3].asset %}
            <td>{{ asset }}</td>
            {% endfor %}
        </tr> 
        <tr class="item">
            <td class="attr">Hashrate (Single Chip)</td>
            {% for val in cooldog[4].single %}
            <td>{{ val }}</td>
            {% endfor %}
        </tr> 
        <tr class="item">
            <td class="attr">Hashrate (Complete Machine, 108Chips)</td>
            {% for val in cooldog[5].total %}
            <td>{{ val }}</td>
            {% endfor %}
        </tr> 
    </table>
    <p style="font-size:20px; color: #333333; margin-top: 20px;">Details of chip performance. More algorithm will be added to the chip and revealed to the public gradually</p>
</div>
<div class="row asic">
    <p class="name">PANOKESON II</p>
    <div class="row" style="width: 1142px; margin: 0 auto;">
        <div> 
            <table style="border: 0px; width:523px; float: left; margin-left: 30px">
                <tr class="item">
                    <td class="attr">Specification</td>
                    <td class="attr">Data</td>
                </tr>
                <tr></tr>
                <tr class="item">
                    <td>Hash Power</td>
                    <td>355 TH/s</td>
                </tr>
                <tr class="item">
                    <td>Power Consumption</td>
                    <td>29.3kW+5%</td>
                </tr>
                <tr class="item">
                    <td>Power Efficiency</td>
                    <td>0.083 J/GH+5% (With proper PSU at 25℃ room temp.)</td>
                </tr>
                <tr class="item">
                    <td>Input Power</td>
                    <td>133A/AC 220V</td>
                </tr>
                <tr class="item">
                    <td>Number of ASIC chips</td>
                    <td>2,600</td>
                </tr>
                <tr class="item">
                    <td>Cooling Method</td>
                    <td>3M Two-phase immersion cooling</td>
                </tr>
            </table>
            <img src="/assets/img/panokseon_01m02.png" style="width: 549px; float: right"/>
            <img src="/assets/img/panokseon_01m03.png" style="width: 523px; float: left"/>
        </div>        
    </div>
</div>
