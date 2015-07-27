索尼活动

编写时间：20150720
测试时间：20150720
上线时间：20150721

   测试数据表：sonycampaign20150701
   测试域名：  dev.iprotime.com



   端口：8039

   正式域名：chinajoy.iprotime.com

   地址： chinajoy.iprotime.com/sonyjoy201507

   图片路径：chinajoy.iprotime.com/sonyjoy201507/images/58612163.jpg

   状态接口：chinajoy.iprotime.com/sonyjoy201507/joy/status



正式数据表：sonyjoy201507



sony  活动
接口说明：

    1.眼睛体验表单提交方式接口：
        提交方式： post
        路径：http://chinajoy.iprotime.com/sonyjoy201507/joy/upload
        提交参数：
            name（姓名 必须）,
            sax（性别）,
            age（年龄 ）,
            mobile（手机 唯一 必须）,
            city  (城市  必须),
            email（邮箱 必须）,
            product_id (产品码 ),
            joinDate（日期 必须）,
            joinTime（时间 必须）,
            img（图片 必须）

        提交成功返回（json格式）：
             {'status': 'success', code: 1,url: '','message': '提交成功'}

        提交失败返回（json格式）：
            {'status': 'error', 'code': '0', 'message': '网络问题，请稍后重试'}
            {'status': 'error', 'code': '2', 'message': '只支持图片格式'}
            {'status': 'error', 'code': '3', 'message': '手机号不能为空'}
            {'status': 'error', 'code': '4', 'message': '手机重复提交'}
            {'status': 'error', 'code': '5', 'message': '邮箱不能为空'}
            {'status': 'error', 'code': '6', 'message': '日期不能为空'}
            {'status': 'error', 'code': '7', 'message': '时间不能为空'}
            {'status': 'error', 'code': '8', 'message': '城市不能为空'}

    2.cl报名提交方式接口：
        提交方式： post
        路径：http://chinajoy.iprotime.com/sonyjoy201507/joy/upload2
        提交参数：
            name（姓名 必须）,
            sax（性别）,
            age（年龄 ）,
            mobile（手机 唯一 必须）,
            email（邮箱 必须）,
            joinDate（日期 必须）,
            img（图片 必须）

        提交成功返回（json格式）：
             {'status': 'success', code: 1,url: '','message': '提交成功'}

        提交失败返回（json格式）：
            {'status': 'error', 'code': '0', 'message': '网络问题，请稍后重试'}
            {'status': 'error', 'code': '2', 'message': '只支持图片格式'}
            {'status': 'error', 'code': '3', 'message': '手机号不能为空'}
            {'status': 'error', 'code': '4', 'message': '手机重复提交'}
            {'status': 'error', 'code': '5', 'message': '邮箱不能为空'}
            {'status': 'error', 'code': '6', 'message': '日期不能为空'}



    3.登录接口：
            提交方式：get
            路径：/chinajoy.iprotime.com//sonyjoy201507/joy/admin/api/login
            用户名：root   密码：1q2w3e


    3.眼睛体验的下载接口：
            提交方式：get
            路径：/chinajoy.iprotime.com//sonyjoy201507/joy/admin/api/downConsumers
            用户名：root   密码：1q2w3e

    3.cl报名下载接口：
            提交方式：get
            路径：/chinajoy.iprotime.com//sonyjoy201507/joy/admin/api/downRecords
            用户名：root   密码：1q2w3e




