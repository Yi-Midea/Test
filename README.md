该项目为4A项目组开发和维护的同步工具，在此做统一管理
该项目包括以下模块：
<table>
    <tr>
        <td>项目名称</td>
        <td>中文名称</td>
        <td>项目描述</td>
    </tr>
    <tr>
        <td>PrivilegeCleanupTool</td>
        <td>权限清理工具</td>
        <td>用于权限清理</td>
    </tr>
	<tr>
        <td>ContactsMySQLSyncTool</td>
        <td>通讯录MySQL同步工具</td>
        <td>通讯录同步工具</td>
    </tr>
    <tr>
        <td>WeakPasswdScanTool</td>
        <td>弱密码扫描工具</td>
        <td>弱密码扫描工具</td>
    </tr>
	<tr>
        <td>mideaidm-login</td>
        <td>用户管理工具</td>
        <td>
			<br>1.用户管理：账号创建、批量创建内部用户;账号编辑、删除、密码重置、启用禁用、设置兼职;组织新建、删除、编辑、移动、映射、委托管理;上网、VPN、邮件、cpc、群组授权管理;机电ERP、OBS、GERP、GSRM、GAPS用户入岗、离岗操作;内部用户HR信息同步、个人通讯录查看、改变内部用户类型、清空密保手机、密保问题
			<br>2.群组管理：群组分类添加、删除、移动;群组创建、成员管理、委托管理、移动、删除;群组按类型可分静态组、动态组;动态组可分原子组、非原子组（原子组可手动添加用户）;群组按功能可分AD群组、邮件群组、普通应用群组、IDM流程自动化群组
			<br>3.统计报告：统计所选部门下，各种类型用户数量
			<br>4.审计报告：审计查询-》用户、组织、群组、职位各种操作类型（例如：添加，删除，修改，禁用，启用用户；重置密码，修改密码；添加删除密保；添加或取消组织映射等）的审计；邮件查询-》流程自动化账号创建、密码过期、密码重置、账号到期、权限添加、权限禁用、供应商账号申请、供应商密码重置、经销商账号申请历史用户查询--》查询历史
			<br>5.系统设置：二级管理员属性显示配置、集成配置属性配置;IDM群组授权管理、超管、二级管理员、IDM访问权限、上网管理权限、icewarp管理权限、vpn管理权限、mip管理权限；ehr与LDAP同步映射字段管理、用户ehr信息同步程序同步管理控制
			<br>6.账号申请：内部，内部临时，职能，外部，IT供应商账号申请;账号变更：账号启用；账号即刻禁用；账号过期时间调整；密保手机，密保问题清空;权限申请及取消：邮件系统权限，上网权限，BI权限，VPN权限；美的部门邮件群发权限
			<br>7.添加供应商账号接口;修改供应商账号接口：当供应商用户存在时，修改供应商的信息；供应商不存在时，创建供应商;禁用供应商账号接口：可以禁用供应商，如果该midea-gsrmcode,midea-gerpcode,midea-gapscode值为1，将以上code值都设置为0;启用供应商账号接口：可以启用供应商，同时清空账号过期时间，默认开通GSRM，GERP权限（即将midea-gsrmcode,midea-gerpcod值设置为1）;重置供应商密码接口：可以发送重置密码链接到用户的邮箱，用户通过点击重置密码链接重置密码。
			<br>8.添加、修改、启用、禁用经销商账号接口;重置经销商密码接口：按照密码强度重置用户的LDAP密码;返回密码过期天数接口：密码倒计时，提醒用户密码还有多少天将过期;返回用户信息接口：通过uid返回用户的基本信息。
			<br>9.产业链账号接口
			<br>10.售后帐号接口
		</td>
    </tr>
	<tr>
        <td>mideaidm-ess</td>
        <td>信息、安全、权限等小工具</td>
        <td>
			<br>1.我的信息：查看基本信息；修改兴趣爱好，工作描述，技能；修改联系信息（为用户提供英文名、账号别名（只能设置一次），修改基本通讯信息，例如：电话、手机、短号、传真等等）
			<br>2.安全中心：修改密码（有密码策略用户，3次内密码不能重复);绑定或解绑密保手机，密保问题；证书管理；账号动态查看；用户自助申请临时访客账号
			<br>3.权限申请：我的权限，权限目录，推荐权限
			<br>4.我的下属：下属成员查看，下属权限信息查看
			<br>3.权限申请：我的权限，权限目录，推荐权限
		</td>
    </tr>
    <tr>
        <td>mideaidm-txl</td>
        <td>通讯录工具</td>
        <td>
			<br>1.企业通讯录：内部组织架构查询，用户查询（通过姓名、邮件地址、账号、手机号码、固定电话、沟通名进行查询）；用户详细信息查看（用户的联系信息，部门，账号，员工编号，职位，兼职部门，职位等）
			<br>2.公共通讯录
			<br>3.个人通讯：个人通讯录、共享通讯录、委托通讯录；个人通讯录是在用户自助上进行维护
		</td>
    </tr>
	<tr>
        <td>mideaidm-hr-sync</td>
        <td>数据同步工具</td>
        <td>
			<br>1.数据同步：内部账号变更同步；内部临时转为内部同步(条件：ldap中证件类型、证件号码、国籍与ehr中一致)；离职禁用，会将用户放到丢失组织节点下，同时修改账号的过期时间，禁用用户相应的职责；组织，岗位新增，修改，删除同步；
			<br>2.后置处理程序：根据岗位计算上级经理
		</td>
    </tr>
	<tr>
        <td>mideaidm-o-sync</td>
        <td>将ehr视图中用户同步到o=sup节点同步工具</td>
        <td>用途O类员工PC端查询薪资信息，同步范围：(O类视图全集)-(ou=employeeO,o=sup下O类员工)</td>
    </tr>
	<tr>
        <td>midea-mobileotype-sync</td>
        <td>将O类视图中用户同步到外部LDAP</td>
        <td>用于O类用户移动端自助查询</td>
    </tr>
	<tr>
        <td>mideaidm-ldaptree</td>
        <td>将内部LDAP扁平化同步为LDAP树状化工具</td>
        <td>将内部LDAP扁平化同步为LDAP树状化，代理上网同步树状化LDAP</td>
    </tr>
	<tr>
        <td>mideaidm-mobileservice</td>
        <td>手机服务端工具</td>
        <td>
			<br>1.添加用户接口，可以在外部LDAP中新增用户。
			<br>2.校验用户是否存在接口，可以判断用户在LDAP中是否存在。
			<br>3.删除外部LDAP用户接口，可以删除外部LDAP中的用户。
			<br>4.禁用用户接口，可以禁用外部LDAP中的用户。
			<br>5.启用用户接口，可以启用外部LDAP中的用户。
			<br>6.查询用户信息接口，可以获取用户信息。
			<br>7.短信找回密码接口，可以通过输入正确的身份证和手机号码找回密码。
			<br>8.重置用户密码接口，可以重置用户的密码。
			<br>9.修改用户信息接口，可以修改用户的基本属性。
			<br>10.用户认证接口，可以验证用户的密码是否正确。
		</td>
    </tr>
	<tr>
        <td>mideaidm-tcstore</td>
        <td>TC门店管理工具</td>
        <td>
			<br>1.添加、修改、禁用、启用TC帐号接口 
			<br>2.修改自己的密码、重置店员的密码接口
			<br>3.密码倒计时，可以显示用户还有多少天密码将过期
			<br>4.查询用户信息，可以查询出用户的基本信息。
		</td>
    </tr>
	<tr>
        <td>mideaidm-webservice</td>
        <td>Web服务端工具</td>
        <td>
			<br>1.静态组添加、删除成员接口;断某个指定成员是否存在静态组中;静态组获取所有成员接口
			<br>2.修改、重置密码接口，可以重置用户密码
			<br>3.验证、修改密保手机接口
			<br>4.验证用户接口，获取用户信息接口
			<br>5.添加用户接口，校验用户是否存在接口
			<br>6.删除外部LDAP用户接口;禁用或启用用户接口
			<br>7.用户接口，可以外部LDAP中的用户。
			<br>8.查询用户信息接口;短信找回密码接口;重置、修改用户密码接口;用户认证接口，可以验证用户的密码是否正确。
		</td>
    </tr>
		<tr>
        <td>mideaidm-ssows</td>
        <td>通过该API进行单点登录</td>
        <td>通过该API进行单点登录</td>
    </tr>
		<tr>
        <td>sso-service</td>
        <td>清除cookie</td>
        <td>注销应用时，调用该包发布的链接清除cookie</td>
    </tr>
		<tr>
        <td>mideaidm-ofmws</td>
        <td></td>
        <td></td>
    </tr>
	</tr>
		<tr>
        <td>mideaidm-mip6sso</td>
        <td></td>
        <td></td>
    </tr>
	</tr>
		<tr>
        <td>mideaidm-mip8sso</td>
        <td></td>
        <td></td>
    </tr>
	</tr>
		<tr>
        <td>mideaidm-miptai6</td>
        <td></td>
        <td></td>
    </tr>
	</tr>
		<tr>
        <td>mideaidm-miptai8</td>
        <td></td>
        <td></td>
    </tr>
	</tr>
		<tr>
        <td>ChangeEBSPwd</td>
        <td>批量重置EBS类账号的密码</td>
        <td>ojdbc修改数据，成功后发送SpringMail</td>
    </tr>
	</tr>
		<tr>
        <td>adorgsync</td>
        <td>新增/修改/移动组织同步工具</td>
        <td></td>
    </tr>
	</tr>
		<tr>
        <td>activityDirectorySynchDelete</td>
        <td>删除组织同步工具</td>
        <td></td>
    </tr>
	</tr>
		<tr>
        <td>adorgsynclostusers</td>
        <td>扫描丢失组织节点下的组织、用户同步工具</td>
        <td></td>
    </tr>
	</tr>
		<tr>
        <td>DisableAndDeleteAccount</td>
        <td>账号到期禁用工具</td>
        <td>
			<br>1.账号到期后，禁用OIM中用户和相应的资源
			<br>2.账号到期3个月后：查询出过期三个月,并且状态为Disabled的所有用户；首先判断该用户是否有ERP权限，如果有，只对AD做删除，其他资源禁用；没有ERP权限的用户，先将用户的基础权限记录到审计库,将用户的静态组权限清除,将用户（内部用户）移到历史节点(历史节点uid命名规则为:H+时间戳+_uid),将OIM中用户的ADLocation值在原来的基础上加D。最后将用户的LDAP和AD资源撤销
		</td>
    </tr>
	</tr>
		<tr>
        <td>LDAPGroupToADGroup</td>
		<td>通过群组去处理LDAP与AD成员不一致工具</td>
        <td>
			<br>1.根据群组cn查询出LDAP中的成员，查出AD中的成员；
			<br>2.对比ldap组和AD组的用户，把ldap组有而Ad组没有的用户添加到AD组；
			<br>3.对比ldap组和AD组的用户，把ldap组没有而Ad组有的用户从Ad组删除
		</td>
    </tr>
	</tr>
		<tr>
        <td>DeleteUser</td>
        <td>删除用户工具</td>
        <td></td>
    </tr>
	</tr>
		<tr>
        <td>prefillorgdn</td>
        <td></td>
        <td></td>
    </tr>
	</tr>
		<tr>
        <td>MideaTools</td>
        <td></td>
        <td></td>
    </tr>
	</tr>
		<tr>
        <td>GERPScheduler</td>
		<td>禁用启用SRM用户工具</td>
        <td>用户回收到OIM后，将用户推送到SRM（并将SRM系统中员工与用户关联）；禁用启用SRM用户职责等操作的EBS如下：
			<br>JDERP：EBS Application Instance
			<<br>OBS：OBSUSERAPP
			<<br>GERP：GERPUSERAPP
			<<br>GSRM：GSRMUSERAPP
			<<br>GAPS：GAPSUSERAPP
        </td>
    </tr>
</table>
