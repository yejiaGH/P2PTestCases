P2P测试用例

1. 打开网站首页，判断是否是该站点
URL: https://www.niwodai.com

2. 判断是否已登录
查询DOM节点：
未登录
<a href="https://member.niwodai.com/login.html" class="mar_l10 toplogin" title="登录">请登录</a>

3. 点击登录链接，跳转到登录页面
URL: https://member.niwodai.com/login.html

4. 登录表单输入用户名、密码、点击登录按钮
4.1 用户名输入框DOM节点
<input type="text" name="username" id="username" class="input_1 pos_u gray_border wid_258">
4.2 密码输入框DOM节点
<input type="password" name="pwd" id="pwd" class="input_1 pos_p gray_border wid_258">
4.3 登录按钮DOM节点
<input type="button" class="submit wid_310" value="登录" id="userLoginBtn">

5. 登录成功以后，自动跳转到账户中心页面
https://member.niwodai.com/member/Investors.html

6. 检查账户余额，>50元即可投资
余额的DOM节点
<em class="mar_r0 fs_28 fc_3 Numfont" id="accAmount">9,900</em>

7. 跳转到投资页面
URL: https://member.niwodai.com/xiangmu

8. 筛选0～1个月
DOM节点
<label for="a5" class="" id="atimetype"><input class="input" type="checkbox" value="0,1">0~1个月</label>
如果$('#atimetype') ,取第1个
筛选行的DOM节点
<div class="fl line_1">
    <label for="a5" class="cur" id="atimetype"><input class="input" type="checkbox" value="0,1">0~1个月</label>
    <label for="a5" class="" id="atimetype"><input class="input" type="checkbox" value="2,3">2~3个月</label>
    <label for="a6" class="" id="btimetype"><input class="input" type="checkbox" value="4,5,6">4~6个月</label>
    <label for="a7" class="" id="ctimetype"><input class="input" type="checkbox" value="7,8,9,10,11,12">7~12个月</label>
    <label for="a8" class="" id="dtimetype"><input class="input" type="checkbox" value="-2">12个月以上</label>
</div>

9. 升序排列
<a href="javascript:;" id="deadline" class="down">期限<i></i></a>

10. 一条项目的DOM结构
<div class="mb_10 item_out">
    <div class="add_bor item_pos_box">
        <span class="b_jingdu b_jd0">
        0%</span>
        
          <a target="_blank" href="/xiangmu/v-ADZUNlYwVTkFY1RgUDJeYQo2VWYCYgJlBTEFPQBjU2A=.html" class="btn btnSize_1 btn_orange mt_5">立即投标</a>
    </div>
    <div class="clearfix module item_in" onclick="window.open('/xiangmu/v-ADZUNlYwVTkFY1RgUDJeYQo2VWYCYgJlBTEFPQBjU2A=.html','_blank')">
        <div class="l">
            <h3 class="tit">
                <i class="ico_all size24 img_icon sItem_12100" title="网络信用标"></i>
                <span class="fc_9">
                    快速短期小额借款
                </span>
                <i class="ico_all size22 img_icon bao_pos mr_10 ml_10"></i><em class="fc_9">适用本金保障计划</em>
                <!--<i class="ico_all size22 img_icon ben_pos3"></i>
                <i class="ico_all size22 img_icon xi_pos3"></i>-->
            </h3>
            <ul class="clearfix item_con">
                <li class="w1">
                    <span class="fc_6">借款年利率</span>
                    <span class="airal fc_orange fs_28">10</span>
      <span class="fc_orange">%</span>                       
                </li>
                <li class="w2">
                    <span class="fc_6">投资期限</span>
                    <span class="airal fs_30">14</span>
                    <span>天</span>
                </li>
                <li class="w3">
                    <span class="fc_6">投资金额</span><!--计划金额 剩余金额-->
                    <span class="airal fs_20">300.00</span>
                </li>
            </ul>
        </div>
        
    </div>
</div>

10.点击进度<100%的项目的立即投标按钮
<div class="add_bor item_pos_box">
    <span class="b_jingdu b_jd0">
    0%</span>
    
      <a target="_blank" href="/xiangmu/v-ADZUNlYwVTkFY1RgUDJeYQo2VWYCYgJlBTEFPQBjU2A=.html" class="btn btnSize_1 btn_orange mt_5">立即投标</a>
</div>