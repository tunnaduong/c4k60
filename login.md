---
layout: default
title: Đăng nhập
permalink: /login/
log: active
---
<h3><i class="fas fa-sign-in-alt"></i> Đăng nhập</h3>
<br>
<div class="wrap-login100">
				<form class="login100-form validate-form" action="authenticate.php" method="POST">
					<span class="login100-form-title p-b-26">
						Sign in to continue
					</span>
					<div class="wrap-input100 validate-input" data-validate="Valid email is: a@b.c">
						<input class="input100" type="text" name="username">
						<span class="focus-input100" data-placeholder="Username"></span>
					</div>
					<div class="wrap-input100 validate-input" data-validate="Enter password">
						<span class="btn-show-pass">
							<i class="zmdi zmdi-eye"></i>
						</span>
						<input class="input100" type="password" name="password">
						<span class="focus-input100" data-placeholder="Password"></span>
					</div>
					<div class="container-login100-form-btn">
						<div class="wrap-login100-form-btn">
							<div class="login100-form-bgbtn"></div>
							<button class="login100-form-btn">
								Login
							</button>
						</div>
					</div>
				</form>
				<center style="padding-top:20px;"><a href="register.html">Don't have an account? Sign up here...</a></center>
			</div>
                        <br>