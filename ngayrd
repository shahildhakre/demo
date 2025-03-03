<div class="form-group" *ngIf="!isLoginMode">
        <label for="confirmPassword">Confirm Password <span class="required">*</span></label>
        <input
          type="password"
          id="confirmPassword"
          formControlName="confirmPassword"
          placeholder="Confirm Password"
          [class.is-invalid]="(authForm.get('confirmPassword')?.invalid || authForm.hasError('passwordMismatch')) && 
            (authForm.get('confirmPassword')?.dirty || authForm.get('confirmPassword')?.touched)"
        />
        <div class="error-icon" *ngIf="authForm.hasError('passwordMismatch') && 
          (authForm.get('confirmPassword')?.dirty || authForm.get('confirmPassword')?.touched)">
          ✕
        </div>
      </div>

      <div class="form-actions">
        <div *ngIf="isLoginMode">
          <span class="signup-link">Don't have an account? <a routerLink="/signup">Sign Up</a></span>
        </div>
        <button type="submit" [disabled]="authForm.invalid" class="sign-btn">
          {{ isLoginMode ? 'Sign In' : 'Sign Up' }}
        </button>
      </div>
    </form>

    <div *ngIf="errorMessage" class="error-message">
      {{ errorMessage }}
    </div>
  </div>
</div>
