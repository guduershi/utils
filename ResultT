import java.io.Serializable;

/**
* @Description:    java封装返回实体类
* @UpdateRemark:   修改内容
* @Version:        1.0
*/
public class ReturnT<T> implements Serializable {

    public static final int SUCCESS_statusCode = 200;
    public static final int FAIL_statusCode = 500;

    /**
     * 返回码
     */
    private int statusCode;
    /**
     * 返回信息
     */
    private String msg;

    /**
     * 返回内容
     */
    private T content;

    public ReturnT(){}

    public ReturnT(int statusCode, String msg){
        this.statusCode = statusCode;
        this.msg = msg;
    }

    public ReturnT(int statusCode, String msg,T content){
        this.statusCode = statusCode;
        this.msg = msg;
        this.content = content;
    }

    public int getstatusCode() {
        return statusCode;
    }

    public void setstatusCode(int statusCode) {
        this.statusCode = statusCode;
    }

    public String getMsg() {
        return msg;
    }

    public void setMsg(String msg) {
        this.msg = msg;
    }

    public T getContent() {
        return content;
    }

    public void setContent(T content) {
        this.content = content;
    }

    public static ReturnT success(String msg, Object object){
        return  new ReturnT(SUCCESS_statusCode,msg,object);
    }

    public static ReturnT fail(String msg){
        return  new ReturnT(FAIL_statusCode,msg);
    }

    @Override
    public String toString() {
        return "ReturnT{" +
                "statusCode=" + statusCode +
                ", msg='" + msg +
                ", content=" + content +
                '}';
    }
}
